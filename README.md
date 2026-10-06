# Super Auto-building agents

Build and continue agents from your goals through Super and your connected Mac app or Chrome extension. The plugin includes the build-agents skill, the Super remote MCP connection, and a reusable Amazon checkout template. Execution requires a Super account and a connected Super client.

## Connect

Enable the plugin and authenticate the Super MCP connection through OAuth at https://app.getsupers.com/mcp. Sign into your Super client with the same account. Claude discovers your connected devices and their current capabilities before running a task. Browser authoring and actions use the model selected in the Super chat interface.

Ask: “Build an agent that researches a topic using my connected Super Chrome extension.” To continue a task, ask Claude to read your existing project and its progress. Completion is reported from observed execution results.

## Walkthrough and template

[Watch the recorded Amazon checkout walkthrough](https://app.getsupers.com/web/plugin-demos/amazon-checkout-walkthrough-20261005.mp4). The demo uses pencils and stops on the checkout payment selection screen without confirming payment or placing an order. Personal address and payment information is masked in the recording.

The bundled Amazon template accepts a product query and quantity, reuses a matching active cart item, preserves unrelated items, and stops before purchase confirmation. The model adapts to observed page state. A generated script alone does not prove successful execution.

## Data and permissions

The declared Super MCP connector sends task prompts, project/chat content, selected device identifiers, generated scripts, and execution results to the Super service. Connected clients can read or interact with websites and local applications within the user's authorized task; those results can contain personal data. Super may route model requests to model providers used by the selected model. Projects and chat history persist to support continued agents. Refer to the [privacy policy](https://app.getsupers.com/privacy) for data handling and retention. The plugin does not install hooks, change Claude permissions, or bundle an executable. OAuth secrets and reviewer credentials are not included.

External sends, purchases, deletions, and other consequential operations require authorization within the user's request. Only the authenticated user's devices and projects may be accessed.

[Support](https://getsupers.com/contact) · [Terms](https://app.getsupers.com/terms). Plugin use is subject to the included LICENSE and Super's terms.
