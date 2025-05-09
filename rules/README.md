## How to Install and Use These Rules in Cursor

1.  **Open Cursor Settings:** Go to `File` > `Settings` (or use the shortcut `Cmd+,` on macOS / `Ctrl+,` on Windows/Linux).
2.  **Navigate to Rules:** In the Settings view, go to `AI` -> `Chat` -> `Custom Rules`.
3.  **Add a New Rule:** Click the `Add Custom Rule` button.
4.  **Copy Rule Content:** Open the desired `.md` file from this folder (e.g., `ReportDrafting_CursorRule.txt`) and copy its *entire* content.
5.  **Paste into Cursor:** Paste the copied text into the large text box provided for the rule definition in Cursor.
6.  **Name the Rule:** Give the rule a descriptive name in Cursor's "Name" field. We recommend using:
    *   `Vulnerability Report Drafter` (for `ReportDrafting_CursorRule.md`)
    *   `PoC Generator` (for `PoC_Generation_CursorRule.md`)
7.  **Save the Rule:** Click the `Save` button (or similar confirmation).
8.  **Repeat:** Repeat steps 3-7 for any other rules you want to add.

**Activating a Rule:**

You can activate a custom rule in two main ways:

*   **Set as Default:** In the `AI` -> `Chat` -> `Custom Rules` settings, you can choose one rule to be the default for all new chat sessions (`⌘+L` or `Ctrl+L`). The `Vulnerability Report Drafter` is a good candidate for the default if you primarily use Cursor for report writing.
*   **Select Manually:** In any AI chat window within Cursor, there's usually a dropdown menu or button (often near the model selection) that allows you to choose which rule to apply for *that specific chat session*. This is useful for switching between the `Vulnerability Report Drafter` and the `PoC Generator` as needed.

## Workflow Integration

*   Use the **`Vulnerability Report Drafter`** rule when following the main workflow: select a comment, start a chat (`⌘+L`), paste a template from the root directory, and add context (`@`).
*   Use the **`PoC Generator`** rule when you need specific, focused help on *just* the Proof of Concept. You might select the vulnerability description comment/text and start a chat with this rule active.

## Important Considerations

*   **AI Output is a Draft:** Always treat the AI's output generated using these rules as a *first draft*. Thoroughly review, verify, edit, and test the generated report sections and especially any PoCs before submission.
*   **Model Choice:** The effectiveness of these rules can depend on the underlying AI model.
*   **Iteration:** Don't hesitate to iterate within the chat. If the first output isn't perfect, provide corrections or ask for refinements (e.g., "Generate the PoC using Foundry," "Make the impact statement more concise," "Focus on X aspect").

---
*These rules aim to enhance the report writing process but require human oversight and expertise.*
