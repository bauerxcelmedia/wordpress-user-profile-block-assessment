# 💻 Technical Assessment: WordPress User Profile Card Block

## Project Overview

The goal of this project is to create a WordPress plugin that provides a **dynamic Gutenberg block**. This block will fetch data from a public API, store the relevant information, and display it on the front end of a WordPress site.

This test is designed to assess your skills in **PHP**, **WordPress development**, **React**, and **modern JavaScript**, as well as your ability to work with external APIs and manage data within the WordPress ecosystem.

---

## The API

For this project, you will be using the **JSONPlaceholder API**, a free-to-use fake online REST API for testing and prototyping.

Specifically, you will be working with the `/users` endpoint: `https://jsonplaceholder.typicode.com/users`

This endpoint returns an array of 10 user objects, each with details like name, email, company, and address.

---

## Core Requirements

Your task is to build a WordPress plugin that, when activated, registers a new Gutenberg block called **"User Profile Card"**.

### 1. Gutenberg Block Functionality

#### Editor View (React):

* The block's editor view should feature a **dropdown menu** that is populated with the names of the users fetched from the JSONPlaceholder API.
* When a user is selected from the dropdown, the block should display a **preview** of their information within the editor (e.g., name, email, and company name).
* The block must save the selected user's **ID** as a block attribute.

#### Front-End View (PHP/React):

* On the front end of the site, the block should render a **"card"** displaying the details of the user selected in the editor.
* The card must display the user's:
    * **Full Name**
    * **Email Address**
    * **Company Name**
    * **Website**
* The rendering of the block on the front end can be done via a **PHP `render_callback`** or dynamically with **React**. Please be prepared to discuss why you chose your approach.

### 2. Technical Specifications

* **Plugin Structure:** The entire project should be contained within a standard WordPress plugin. Please include a main plugin file with the necessary headers.
* **Data Fetching:** The API call to fetch the user data should be made from the block's **edit component in React**.
* **Error Handling:** The block should gracefully handle potential API errors. For instance, if the API is unavailable, the editor view should display an **appropriate message** to the user.
* **Styling:**
    * Apply some **basic styling** to the user profile card on the front end to make it visually appealing.
    * A simple, clean design is sufficient. Feel free to use the default WordPress component styles in the editor.

---

## What We're Looking For

* **Clean, Readable Code:** Your code should be well-organized, commented where necessary, and easy to understand.
* **Best Practices:** Adherence to WordPress and React best practices.
* **Problem-Solving:** A logical approach to fetching, storing, and displaying data.
* **Completeness:** A functional plugin that meets all the requirements.

---

## A Note on Using AI

We recognize that AI tools are a standard part of modern development workflows. You are **not prohibited** from using AI assistants (like GitHub Copilot, ChatGPT, etc.) to help you with this test.

However, our goal is to understand your problem-solving process and coding proficiency. If you use an AI tool, please adhere to the following guidelines:

* **Acknowledge Usage:** In your code, leave a comment indicating which parts were generated or influenced by an AI assistant.
* **Share Your Prompts:** In your Pull Request description, include a section with the prompts you used.
* **Be Prepared to Explain:** You are responsible for all code you submit. Be prepared to explain the logic, justify the approach, and discuss any trade-offs, regardless of whether you wrote it from scratch or used an AI to generate it.

---

## Submission Instructions (Revised)

To best simulate our real-world development workflow, we'd like you to submit your work via a **pull request**.

1.  **Use Our Template:** We will provide a link to a public GitHub template repository for this test.
2.  **Create Your Private Repository:** Use the template to create your own **private repository** for your submission. (Note: GitHub offers free private repositories for all users). Please **do not fork** the template repository directly.
3.  **Grant Access:** Invite the relevant GitHub user(s) (we will provide the usernames) as **collaborator(s)** to your private repository so we can review your work.
4.  **Develop on a Branch:** Create a new feature branch for your work (e.g., `feature/user-profile-block`).
5.  **Commit Your Changes:** Make **small, logical commits** as you build the plugin. Write clear and concise commit messages.
6.  **Update the README:** Edit the README.md file in your repository to include clear instructions on how to install and use your plugin. Be sure to document any required build steps (e.g., `npm install` and `npm run build`).
7.  **Open a Pull Request:** When you have completed the test, open a pull request in your private repository to merge your feature branch into your main branch.
    * Write a clear title and a brief description for your pull request, explaining your approach, any trade-offs you made, and any other notes for the reviewer. **This description must also include clear installation and usage steps** (e.g., `npm install` and `npm run build`).
8.  **Notify Us:** Once the pull request is open, please **email us a link** to it.

This process allows us to review your code, your Git practices, and your communication style—all essential skills for collaborating on our team.

We look forward to seeing your work!