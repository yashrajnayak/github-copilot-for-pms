## Step 3: Multi-File Feature Development with AI

Now let's explore one of Copilot's most powerful capabilities for product development: making coordinated changes across multiple files to implement new features. This is where AI really shines in accelerating product delivery.

### Understanding Copilot Edits from a Product Perspective

[Copilot Edits](https://code.visualstudio.com/docs/copilot/copilot-edits) represents a significant leap in AI-powered development. Instead of making small, isolated changes, it can implement complete features that span multiple files - exactly what product managers need for rapid feature delivery.

#### Business Benefits

- **Faster feature delivery**: Complete features implemented in minutes, not hours or days
- **Consistent implementation**: AI ensures all related files are updated cohesively
- **Reduced coordination overhead**: No need to manually track which files need updates
- **Lower risk of errors**: AI maintains consistency across the entire feature implementation

#### How It Works (Business View)

1. **Define scope**: Select which files should be part of the feature implementation
2. **Describe requirements**: Use natural language to explain what you want to build
3. **Review changes**: See all proposed changes across files before accepting
4. **Iterate**: Provide feedback to refine the implementation

### :keyboard: Activity: Implement a Complete Feature with AI 🚀

Let's add a new feature that displays current participants for each activity - a common request from stakeholders who want better visibility into program engagement.

1. Switch the Copilot Chat panel to **Edit** mode using the dropdown at the bottom.

   <img width="350" alt="image" src="https://github.com/user-attachments/assets/646fc94a-7d60-4821-b9cf-9ec6f4fd03d7" />

2. Add the relevant files to the working set by dragging them to the chat panel:

   - `src/static/app.js` (handles user interactions)
   - `src/static/index.html` (page structure)
   - `src/static/styles.css` (visual design)

   **Product Insight**: This step defines the scope of our feature - AI will coordinate changes across all these files.

3. Describe the feature requirement in business terms:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > Add a participants section to each activity card that shows who is currently signed up. 
   > Display the participants as a clean, bulleted list. Make sure it looks professional 
   > and fits well with the existing design.
   > ```

   **Key Point**: Notice how we can describe requirements in product language, focusing on user experience rather than technical implementation.

4. Watch as AI proposes changes across multiple files simultaneously. You'll see:
   - Icons next to file names indicating they have suggested edits
   - A navigation panel to review each change
   - In-context previews of all modifications

      <img width="200" alt="files with icons indicating they have been edited" src="https://github.com/user-attachments/assets/9c7c2e10-cd18-43c5-9947-cffd6dde0473" />

5. **Test the feature** before accepting changes. Restart the application and refresh your browser to see the new participant lists in action.

   <img width="350" alt="Activity card with participant info" src="https://github.com/user-attachments/assets/c4d56187-4791-4c8e-87d7-d5ce7cdc0bee" />

   **Product Validation**: This step demonstrates how you can validate AI-generated features before deployment - crucial for maintaining quality standards.

6. If the feature works as expected, use the navigation panel to review and **Keep** each suggested change.

### Business Impact Analysis

This exercise demonstrates several key advantages of AI-powered development:

**Speed**: A feature that might take a developer 2-3 hours was implemented in minutes
**Coordination**: AI automatically updated HTML structure, JavaScript functionality, and CSS styling
**Consistency**: All changes work together seamlessly without integration issues
**Quality**: The feature follows existing design patterns and coding standards

### :keyboard: Activity: Deploy Your Feature 🚀

1. Commit and push your changes using the Source Control panel.

2. **Optional Advanced Exercise**: Add a comment asking about Agent mode:

   ```txt
   Hey @professortocat, Agent mode sounds interesting for complex features. 
   Can you explain how it might help with larger product initiatives?
   ```

### Key Takeaways for Product Strategy

- **Reduced development cycles**: Features can be prototyped and implemented much faster
- **Lower technical risk**: AI helps maintain code quality and consistency
- **Better stakeholder demos**: Rapid feature implementation enables more frequent demonstrations
- **Increased innovation capacity**: Teams can focus on complex problem-solving rather than routine implementation

This capability fundamentally changes how you can approach product planning and stakeholder management. Features that once required significant development time can now be implemented and tested rapidly.

Wait for Mona to verify your implementation before proceeding!

<details>
<summary>Having trouble? 🤷</summary><br/>

If you don't get feedback, check that:

- You've committed changes to files in the `src/static/` directory
- Changes are pushed to the `accelerate-with-copilot` branch
- The participant feature is visible when you view the website

</details>