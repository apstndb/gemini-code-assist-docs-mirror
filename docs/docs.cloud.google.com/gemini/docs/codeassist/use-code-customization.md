---
name: documents/docs.cloud.google.com/gemini/docs/codeassist/use-code-customization
uri: https://docs.cloud.google.com/gemini/docs/codeassist/use-code-customization
title: Use Gemini Code Assist code customization
description: Describes how to use Gemini Code Assist code customization.
data_source: docs.cloud.google.com
---

This document describes how to use [Gemini Code Assist code customization](https://docs.cloud.google.com/gemini/docs/codeassist/code-customization-overview) and provides a few best practices. This feature lets you receive code recommendations, which draw from the internal libraries, private APIs, and the coding style of your organization.

## Before you begin

1.  [Set up Gemini Code Assist](https://docs.cloud.google.com/gemini/docs/codeassist/set-up-gemini) with an [Enterprise subscription](https://docs.cloud.google.com/gemini/docs/codeassist/overview#supported-features) .

2.  [Set up Gemini Code Assist code customization](https://docs.cloud.google.com/gemini/docs/codeassist/code-customization) .

## How to use code customization

The following table lists ways to use Gemini Code Assist code customization:

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Form</th>
<th>How to trigger</th>
<th>Notes and resources</th>
</tr>
<tr class="odd">
<th><p>Natural language chat</p></th>
<th><p>Enter a natural language prompt in Gemini Code Assist chat in the IDE.</p></th>
<th><p>Consider the following:</p>
<ul>
<li>Chat history is not available. Avoid multi-step queries.</li>
<li>You can ask for more details about sources, including links to the specific sources.</li>
<li>If you highlight or select code when you send a message in chat, Gemini Code Assist uses that code to improve code customization and chat quality.</li>
</ul>
<p>For more information, see <a href="https://docs.cloud.google.com/gemini/docs/codeassist/chat-overview">Chat with Gemini Code Assist</a> .</p></th>
</tr>
<tr class="header">
<th>Generate code</th>
<th>In the quick pick bar in your IDE, either with or without selected code, press <kbd> Command+Enter </kbd> (on macOS) or <kbd> Control+Enter </kbd> .</th>
<th>For more information, see <a href="https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#generate_code_with_prompts">Generate code with prompts</a> .</th>
</tr>
<tr class="odd">
<th>Transform code</th>
<th>In the quick pick bar in your IDE, either with or without selected code, enter <code>/fix</code> .</th>
<th>For more information, see <a href="https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#generate_code_with_prompts">Generate code with prompts</a> .</th>
</tr>
<tr class="header">
<th>Autocomplete</th>
<th>Code customization is automatically triggered and provides suggestions based on what you write.</th>
<th><p>Consider the following:</p>
<ul>
<li>Code completion needs a certain level of confidence to propose a suggestion. Ensure that a substantial amount of code is available so that relevant snippets are retrieved.</li>
<li>Code completion checks if you have required libraries in order to use certain elements of the function.</li>
</ul>
<p>For more information, see <a href="https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#get_code_completions">Get code completions</a> .</p></th>
</tr>
<tr class="odd">
<th>Remote repository context</th>
<th><ol>
<li>Start your prompt with the <kbd> @ </kbd> symbol. A list of available remote repositories that are indexed appears.</li>
<li>Select the repository you want to use for context from the list. You can also start typing the repository name to filter the list.</li>
<li>After selecting the repository, write the rest of your prompt.</li>
</ol></th>
<th><p>Remote repository context is useful when you are working on a task that is mostly related to a specific set of microservices, libraries, or modules.</p>
<p>For more information, see <a href="https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#get_more_relevant_suggestions_with_remote_repository_context">Get more relevant suggestions with remote repository context</a> .</p></th>
</tr>
</thead>

</table>

## Use cases and prompt examples

The following table provides guidance and examples about using code customization in specific use cases:

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Use case</th>
<th>Things worth trying</th>
</tr>
<tr class="odd">
<th>Writing new code</th>
<th><p>Try the following to generate code in your IDE or Gemini Code Assist chat:</p>
<ul>
<li>Generate code that would use terms which are already mentioned in your codebase.</li>
<li>Paste in your code, such as a functional signature or code with <code>TODO</code> comments, and then ask Gemini Code Assist to fill in or replace <code>TODO</code> comments with code. Add comments with explanation from context.</li>
</ul>
<p>Try generating code with the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"Write a main function where a connection to <var translate="no">DATABASE</var> is created. Include health checks."</li>
<li>"Write a <var translate="no">FUNCTION_OR_CLASS</var> in the following structure: <var translate="no">EXPLAIN_STRUCTURE</var> ."</li>
</ul>
<p>After you generate some code, try using a follow-up prompt to improve it:</p>
<ul>
<li>"Try the <code>/fix</code> command to adjust the generated code—for example, syntax errors."</li>
<li>"Add missing imports."</li>
<li>"Try <code>/fix</code> on chat-generated code."</li>
</ul></th>
</tr>
<tr class="header">
<th>Cleaning, simplifying, and refactoring code</th>
<th><p>Try the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"Can you merge <var translate="no">IMPORTS_VARIABLES_OR_NOTE_EXPORTED_FUNCTIONS</var> in this file?"</li>
<li>"How would you simplify the <var translate="no">FUNCTION_NAME</var> function?"</li>
<li>"Can you merge <var translate="no">FUNCTION_NAME_1</var> and <var translate="no">FUNCTION_NAME_2</var> into one function?"</li>
<li>"Could you inline some variables in <var translate="no">FUNCTION_NAME</var> ?"</li>
<li>"Could you simplify variable naming in the function <var translate="no">FUNCTION_NAME</var> ?"</li>
</ul></th>
</tr>
<tr class="odd">
<th>Readability</th>
<th><p>Try the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"Write the function <var translate="no">FUNCTION_NAME</var> in fewer lines of code, if possible."</li>
<li>"Add comments to the function <var translate="no">FUNCTION_NAME</var> ."</li>
<li>"Remove unnecessary whitespaces in the function <var translate="no">FUNCTION_NAME</var> ."</li>
<li>"Format the function <var translate="no">FUNCTION_NAME</var> in a similar way as the rest of the code."</li>
</ul></th>
</tr>
<tr class="header">
<th>Code review</th>
<th><p>Try the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"Split the code in parts and explain each part using our codebase."</li>
<li>"Are there variables or keywords that could be shorter and more self-explanatory?"</li>
<li>"Can you give me useful code from the <var translate="no">REPOSITORY_NAME_PACKAGE_MODULE</var> context for this code?"</li>
<li>"What do you think about the function <var translate="no">FUNCTION_NAME</var> ?"</li>
</ul></th>
</tr>
<tr class="odd">
<th>Debugging</th>
<th><p>Try the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"I am getting an error when I try to do X/add Y. Why?"</li>
<li>"Can you spot an error in the function <var translate="no">FUNCTION_NAME</var> ?"</li>
<li>"How would you fix the function <var translate="no">FUNCTION_NAME</var> given this error message?"</li>
</ul></th>
</tr>
<tr class="header">
<th>Learning and onboarding</th>
<th><p>Try the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"Split this code in parts and explain each of them using our codebase."</li>
<li>"Show how to call function <var translate="no">FUNCTION_NAME</var> ?"</li>
<li>"Show how to run the main function in the <var translate="no">ENVIRONMENT_NAME</var> environment?"</li>
<li>"What is the key technical improvement we can do to make this code more performant?"</li>
<li>"Show me the implementation of <var translate="no">FUNCTION_OR_CLASS_NAME</var> to achieve better results and add what that specific element is"—for example, "Show me the implementation of function foo where foo is the name of the function."</li>
</ul></th>
</tr>
<tr class="odd">
<th>Migration</th>
<th><p>Try the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"Give me a strategy for how I can migrate <var translate="no">FILE_NAME</var> from <var translate="no">LANGUAGE_1</var> to <var translate="no">LANGUAGE_2</var> "—for example, from Go to Python.</li>
<li>"Given the function <var translate="no">FUNCTION_NAME</var> in repository <var translate="no">REPOSITORY_NAME</var> , find me an equivalent function in language <var translate="no">LANGUAGE_NAME</var> that I can use."</li>
</ul>
<p>Try the following chat-based or code generation transformation workflow using prompts:</p>
<ol>
<li>"Take <var translate="no">FILENAME_COMPONENT</var> code already written in <var translate="no">LANGUAGE_1</var> and refactor and migrate it to <var translate="no">LANGUAGE_2</var> "—for example, from Go to Python.</li>
<li>After you migrate some code, try the following:
<ul>
<li>Select smaller chunks and use <code>/fix</code> to get it into a state that you want.</li>
<li>Try the following prompts:
<ul>
<li>"Is there something which can be improved?"</li>
<li>"Give me possible pain points."</li>
<li>"How would you test this code if that migration is correct?"</li>
</ul></li>
</ul></li>
</ol></th>
</tr>
<tr class="header">
<th>Generating documentation</th>
<th><p>Try the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"Summarize the code in package or folder <var translate="no">X</var> and provide documentation for the top five important methods."</li>
<li>"Generate documentation for <var translate="no">FUNCTION_OR_CLASS_NAME</var> ."</li>
<li>"Shorten the documentation while preserving the key information."</li>
</ul></th>
</tr>
<tr class="odd">
<th>Unit test generation</th>
<th><p>Try the following prompts in Gemini Code Assist chat:</p>
<ul>
<li>"Generate unit tests for <var translate="no">FILENAME</var> ."</li>
<li>"Add the most relevant test cases for the <var translate="no">FUNCTION_NAME</var> function."</li>
<li>"Remove test cases that you think don't bring much value."</li>
</ul></th>
</tr>
</thead>

</table>

## Best practices

- **Use relevant variable and function names or code snippets.** This guides code customization towards the most pertinent code examples.
- **Use index repositories that you want to scale, and avoid adding deprecated functionality.** Code customization helps to scale to the code style, patterns, code semantics, knowledge, and implementations across the codebase. Bad examples of repositories to scale are deprecated functionalities, generated code, and legacy implementations.
- **For code retrieval use cases, use code generation functionality instead of code completion** . Prompt using language such as "Using the definition of `FUNCTION_NAME` , generate the exact same function," or "Generate the exact implementation of `FUNCTION_NAME` ."
- **Have includes or imports present in the file for the code that you want to retrieve** to improve Gemini contextual awareness.
- **Execute only one action for each prompt.** For example, if you want to retrieve code and have this code be implemented in a new function, perform these steps over two prompts.
- **For use cases where you want more than just code** (such as code explanation, migration plan, or error explanation), use code customization for chat, where you have a conversation with Gemini with your codebase in context.
- **Note that AI model generation is non-deterministic** . If you aren't satisfied with the response, executing the same prompt again might achieve a better result.
- **Note that generating unit tests** generally works better if you open the file locally, and then from chat, ask to generate unit tests for this file or a specific function.

### **Get more relevant suggestions with remote repository context**

You can get more contextually aware and relevant code suggestions by directing Gemini Code Assist to focus on specific remote repositories. By using the <span class="kbd"> @ </span> symbol in the chat, you can select one or more repositories to be used as a primary source of context for your prompts. This is useful when you are working on a task that is mostly related to a specific set of microservices, libraries, or modules.

To use a remote repository as context, follow these steps in your IDE's chat:

1.  Start your prompt with the <span class="kbd"> @ </span> symbol. A list of available remote repositories that are indexed will appear.
2.  Select the repository you want to use for context from the list. You can also start typing the repository name to filter the list.
3.  After selecting the repository, write the rest of your prompt.

Gemini will then prioritize the selected repository when generating a response.

#### **Example Prompts**

Here are some examples of how you can use this feature:

- **To understand a repository:**
  - " <span class="kbd"> @ </span> `REPOSITORY_NAME` What is the overall structure of this repository?"
  - " <span class="kbd"> @ </span> `REPOSITORY_NAME` I'm a new team member. Can you give me an overview of this repository's purpose and key modules?"
- **For code generation and modification:**
  - " <span class="kbd"> @ </span> `REPOSITORY_NAME` Implement an authentication function similar to the one in this repository."
  - " <span class="kbd"> @ </span> `REPOSITORY_NAME` Refactor the following code to follow the conventions in the selected repository."
  - " <span class="kbd"> @ </span> `REPOSITORY_A_NAME` How can I use the latest functions from this repository to improve my code in `REPOSITORY_B_NAME` ?"
- **For testing:**
  - " <span class="kbd"> @ </span> `UNIT_TEST_FILE_NAME` Generate unit tests for `MODULE` based on the examples in the selected file."

By using remote repositories as a focused source of context, you can get more accurate and relevant suggestions from Gemini Code Assist, which can help you code faster and more efficiently.
