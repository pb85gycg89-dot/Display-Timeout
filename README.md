This AutoIt script provides a graphical user interface (GUI) and command-line tool to manage Windows screen and standby timeouts using the system's powercfg utility.

Key Features

• Graphical User Interface (GUI): Launches a compact, dark-themed window displaying options to quickly change the timeout duration to 5, 15, 30, 60 minutes, or "Never". It also fetches and highlights the current active setting upon opening.
• Command-Line Interface: Operates silently in the background when launched with specific switches:
	• /status: Detects the current power source (AC power vs. battery) via WMI and writes the active timeout configuration to the console.
	• /default: Quietly overrides display and standby timeouts to 15 minutes before closing.
• System Integration: Executes underlying command-line processes (powercfg) to programmatically adjust both monitor-timeout and standby-timeout behaviors for plugged-in (AC) and battery (DC) states.
