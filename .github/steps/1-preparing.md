## Step 1: Understanding GitHub Copilot from a Product Perspective

Welcome to your **"GitHub Copilot for Product Managers"** exercise! 🚀

In this exercise, you'll explore how GitHub Copilot works by observing its impact on a real project - a website for Mergington High School students to sign up for extracurricular activities. 🎻 ⚽️ ♟️

<img width="600" alt="screenshot of Mergington High School WebApp" src="https://github.com/user-attachments/assets/472398fd-1aa1-4084-b443-4e242deb30d9" />

### What is GitHub Copilot and Why Should Product Managers Care?

<img width="150" align="right" alt="copilot logo" src="https://github.com/user-attachments/assets/4d22496d-850b-4785-aafe-11cba03cd5f2" />

GitHub Copilot is an AI coding assistant that helps developers write code faster and with less effort. For product managers, this translates to:

- **Faster time-to-market**: Features can be built and iterated on more quickly
- **Reduced development costs**: Less time spent on routine coding tasks
- **Higher quality output**: AI helps catch bugs and suggests best practices
- **Better developer experience**: Happier, more productive engineering teams

Research shows GitHub Copilot can increase developer productivity by up to 55% and significantly improve developer satisfaction. For more details, see [Research: quantifying GitHub Copilot's impact on developer productivity and happiness](https://github.blog/news-insights/research/research-quantifying-github-copilots-impact-on-developer-productivity-and-happiness/).

### How Teams Interact with GitHub Copilot

Your development teams will primarily use Copilot in these ways:

- **Inline suggestions**: As developers type, Copilot suggests code completions, similar to autocomplete in email but for entire functions
- **Copilot Chat**: A conversational interface where developers can ask coding questions and get tailored responses
- **Copilot Edits**: Allows making changes across multiple files using natural language instructions
- **Copilot Agent**: An advanced mode that can work iteratively to complete complex, multi-step tasks

> [!TIP]
> Understanding these interaction modes helps you better estimate project timelines and communicate with your engineering team about what's possible with AI assistance.

### Business Impact: What This Means for Your Products

As you work through this exercise, consider how AI-assisted development could impact:

- **Feature development velocity**: How much faster could your team ship new features?
- **Technical debt reduction**: AI can help maintain and improve existing code
- **Innovation capacity**: With routine tasks automated, teams can focus on creative problem-solving
- **Quality assurance**: AI assistance can help catch issues before they reach production

### :keyboard: Activity: Set Up Your Development Environment and Explore the Project

Let's start by setting up a development environment and using Copilot to understand our sample project.

1. Left-click the below button to open the **Create Codespace** page in a new tab. Use the default configuration.

   [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/aicodingworkshop/github-copilot-for-pms?quickstart=1)

2. Confirm the **Repository** field is your copy of the exercise, not the original, then click the green **Create Codespace** button.

   - ✅ Your copy: `/{{{full_repo_name}}}`
   - ❌ Original: `/aicodingworkshop/github-copilot-for-pms`

3. Wait a moment for Visual Studio Code to load in your browser. This is a full development environment running in the cloud!

4. In the left sidebar, click the extensions tab and verify that the `GitHub Copilot` and `Python` extensions are installed and enabled.

   <img width="350" alt="copilot extension for VS Code" src="https://github.com/user-attachments/assets/ef1ef984-17fc-4b20-a9a6-65a866def468" />

   <img width="350" alt="python extension for VS Code" src="https://github.com/user-attachments/assets/3040c0f5-1658-47e2-a439-20504a384f77" />

5. At the top of VS Code, locate and click the **Copilot icon** to open a Copilot Chat panel.

   <img width="150" alt="image" src="https://github.com/user-attachments/assets/5e64db46-95cb-415d-badc-b6b8677f10c1" />

6. If this is your first time using GitHub Copilot, you will need to accept the usage terms to continue.

7. Enter the below prompt to ask Copilot to introduce you to the project from a business perspective.

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > @workspace Please explain this project from a product manager's perspective. 
   > What business problem does it solve? What are the key features? 
   > How would I run it to see it in action?
   > ```

   <details>
   <summary>What is @workspace?</summary>
   The @workspace command tells Copilot to analyze the entire project repository to provide context-aware responses. This is particularly useful for understanding project scope and architecture.
   </details>

8. Now let's see the application in action! In the left sidebar, select the `Run and Debug` tab and then press the **Start Debugging** icon.

   <img width="300" alt="image" src="https://github.com/user-attachments/assets/50b27f2a-5eab-4827-9343-ab5bce62357e" />

9. To view the website, expand the lower panel and select the **Ports** tab. Find port `8000` and click the **Open in browser** icon.

   ![image](https://github.com/user-attachments/assets/92d5642e-ce99-4a66-850c-2d311a673596)

### :keyboard: Activity: Use Copilot to Help with Project Management Tasks 📋

Now let's see how Copilot can assist with common project management needs like creating branches for new features.

1. Return to VS Code and open a new terminal by clicking the **Terminal** tab in the bottom panel, then clicking the plus `+` sign.

2. Use the keyboard shortcut `Ctrl + I` (Windows) or `Cmd + I` (Mac) to bring up **Copilot's Terminal Inline Chat**.

3. Ask Copilot to help you set up a new feature branch:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > I need to create a new Git branch for adding features to this project. 
   > What's the best practice for branch naming and how do I create and publish it?
   > ```

4. Copilot will suggest commands. Follow up with a specific request:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > Great! Let's use the branch name "accelerate-with-copilot" 
   > and publish it to the remote repository.
   > ```

5. Click the `Run` button to execute the commands Copilot suggests.

6. Check the VS Code status bar (bottom left) to confirm you're now on the `accelerate-with-copilot` branch.

### Key Takeaways for Product Managers

- **AI reduces friction**: Tasks that might require looking up documentation or asking team members can be completed instantly
- **Natural language interface**: You can communicate with AI tools using business language, not technical jargon
- **Contextual awareness**: AI understands your project context and provides relevant suggestions
- **Iterative refinement**: You can clarify and refine requests, just like working with a team member

Wait for feedback from Mona (our automated assistant) before proceeding to the next step!

<details>
<summary>Having trouble? 🤷</summary><br/>

If you don't get feedback, here are some things to check:

- Make sure you created the branch with the exact name `accelerate-with-copilot`
- Verify the branch was published to your repository
- Check that you're working in your copy of the repository, not the original

</details>