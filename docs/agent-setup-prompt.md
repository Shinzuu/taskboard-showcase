Set up taskboard, a small task-board command for Claude Code, on this computer. Do as much as you can yourself and ask me only for the things you cannot do.

<context>
taskboard is one bash command plus one Claude Code skill. It reads and updates my own tasks on a team's task board through that board's personal task API: list my open tasks, read a task, change status, comment, log time and run the timer. The skill makes Claude show every write and wait for my yes. I received the taskboard folder from its author; it is not downloaded from anywhere. The folder's README describes the install; read it first and follow it. Where it and this prompt disagree, the README wins.

What taskboard needs:
- Claude Code.
- bash, curl, jq and GNU date (on macOS, the GNU date tools from coreutils).
- My own personal API key for the board. It only sees tasks assigned to me.
</context>

<steps>
1. Ask me where the taskboard folder is. Confirm it contains the command, the skill and the offline tests.
2. Check bash, curl, jq and GNU date. Tell me what is missing.
3. Install the command onto my PATH and the skill into my Claude Code skills folder, as the README describes. Show me each path before you write to it.
4. Have me store my key: create the private key file the README names with mode 600, and give me a one-line command that reads the key without echo so I can paste it myself. Never ask me to paste the key into this chat, and never read, print or copy the key.
5. Run the offline tests and report the pass count.
6. Test with the command's "who am I" call and show me only the name it returns.
7. Report what you installed, where, and the results.
</steps>

<rules>
- Read-only on the board during setup. Do not change a status, comment, log time or start the timer.
- If a step fails twice, stop and tell me what you saw instead of trying other routes.
</rules>
