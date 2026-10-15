---
"@signalridge/pi-tab-status": patch
---

Keep the tab in the running state while a tool is still executing, so a long command that emits no intermediate events is no longer reported as blocked. In-flight tool executions are tracked by tool call id and cleared on their end, on settlement, and on session reset.
