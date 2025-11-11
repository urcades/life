# Swift Instructions

1. Never let AI modify .pbxproj files. Create files with Claude Code, add them to Xcode manually. One corrupted project file will waste hours.

2. Document platform gotchas immediately. Hit an iOS 26 API issue? Add it to http://CLAUDE.md that session. "NO .background() before .glassEffect()" saved me from
repeating that mistake 50+ times.

3. Use feature flags for experimental code. Toggle new features on/off without rebuilding. Makes rolling back instant when something breaks at 11pm.

4. Always request debug logging. Ask Claude Code to add Logger statements for complex flows. Future you will thank past you when debugging async camera issues.

5. Test after every change!! Clean build folder (Cmd+Shift+K), run on device, verify in console. Catch issues before they compound.

6. Keep conversations focused on single components. Don't ask to "refactor the whole app" Smaller scope = better results.

7. Document what changed in session. End every major change with a markdown file explaining what broke, how it was fixed, and rollback steps. 
