## Step 2: Seeing AI-Powered Development in Action

In the previous step, you learned about GitHub Copilot's business value. Now let's see how it solves real development challenges that directly impact product delivery!

We've discovered a critical bug: students can register for the same activities multiple times. This creates data integrity issues and a poor user experience. Let's see how Copilot helps identify and fix this problem quickly.

### Understanding the AI Development Process

Before we dive in, let's understand how AI-powered development works from a product perspective:

- **Context is key**: AI performs better when it understands the project structure and business requirements
- **Iterative improvement**: Like working with a team member, you can refine requests and provide feedback
- **Quality assurance**: AI suggestions still need human review, but they dramatically speed up the process
- **Documentation**: AI can explain complex code in business terms

### Business Impact of This Bug Fix

This bug fix demonstrates several key benefits of AI-assisted development:

- **Faster problem identification**: AI can quickly scan code to find potential issues
- **Reduced debugging time**: Instead of manually searching through files, AI pinpoints the problem area
- **Consistent quality**: AI suggests best practices and helps prevent similar issues
- **Knowledge transfer**: AI explanations help team members understand the codebase

### :keyboard: Activity: Watch AI Identify and Fix a Critical Bug 🐛

1. Open the **Copilot Chat** panel and ask it to analyze our business problem:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > @workspace We have a business-critical bug: students can register twice for the same activity. 
   > This creates data problems and confuses users. Where in the code might this issue be occurring?
   > ```

   **Product Manager Insight**: Notice how we can describe the problem in business terms, and AI translates this into technical analysis.

2. Based on Copilot's analysis, let's examine the problematic code. Open the `src/app.py` file from the file explorer.

3. Scroll to the `signup_for_activity` function (around line 50). This is where students register for activities.

4. Let's add a comment to guide the fix and see AI complete the solution:

   ```python
   # Validate student is not already signed up
   ```

5. Press Enter and then Tab to accept Copilot's suggestion for the validation logic.

   **Business Value**: This demonstrates how AI can implement business rules quickly and correctly.

   <details>
   <summary>Example of what Copilot might suggest</summary><br/>

   ```python
   # Validate student is not already signed up
   if email in activity["participants"]:
       raise HTTPException(status_code=400, detail="Student is already signed up")
   ```

   </details>

### :keyboard: Activity: Use AI to Generate Test Data 📊

Product managers often need realistic test data for demos, user testing, and stakeholder presentations. Let's see how AI can help:

1. In the `src/app.py` file, find the `activities` section (around line 23) where sample activities are defined.

2. Click on any line in this section and use `Ctrl + I` (Windows) or `Cmd + I` (Mac) to open inline chat.

3. Request more diverse test data:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > Add 2 more sports activities, 2 more artistic activities, and 2 more academic activities. 
   > Make them realistic for a high school setting with appropriate schedules and participant limits.
   > ```

4. Review the suggestions and click **Accept** if they look good.

   **Product Value**: AI can quickly generate realistic, diverse content for testing and demonstrations, saving significant time in product development.

### :keyboard: Activity: AI-Generated Documentation 📝

Let's see how AI can help with project documentation - crucial for stakeholder communication:

1. In the Source Control tab (left sidebar), stage your changes by clicking the `+` next to `app.py`.

2. Instead of writing a commit message manually, click the **Generate Commit Message with Copilot** button (sparkles icon) next to the message box.

3. Review the AI-generated message and commit your changes.

4. Click **Sync Changes** to push to GitHub.

**Product Manager Insight**: AI can automatically document changes in clear, professional language, making it easier to track feature development and communicate progress to stakeholders.

### Key Business Insights from This Step

- **Rapid problem resolution**: What might take hours of debugging was solved in minutes
- **Quality improvement**: AI suggests best practices and helps prevent future issues
- **Better documentation**: Automatic generation of clear, professional documentation
- **Scalable content creation**: AI can quickly generate realistic test data and content

This demonstrates how AI doesn't just speed up development - it improves quality and reduces the risk of shipping bugs to production.

Wait for Mona to verify your work before proceeding to the next step!

<details>
<summary>Having trouble? 🤷</summary><br/>

If you don't get feedback, check that:

- You've pushed changes to the `src/app.py` file
- Your changes are on the `accelerate-with-copilot` branch
- The file includes the duplicate registration check

</details>