# DevLogger
The purpose of DevLogger is to provide a set of logging functions that are used during the development process in Unity. It allows developers to log messages, warnings, errors, and exceptions only in the Unity Editor, without affecting the performance or adding unnecessary output in the final build when the game is released.

Key Features of DevLogger:
Conditional Logging:

The logging methods are only active when the game is running in the Unity Editor, thanks to the Conditional("UNITY_EDITOR") attribute.

When the game is built and deployed (e.g., for a mobile or standalone platform), the logging calls are automatically excluded from the code, ensuring no performance overhead.

Logging Levels:

Log: For general messages that can help developers understand the flow or state of the game.

LogWarning: For warnings that indicate potential issues or important notes that don't break functionality but should be noticed.

LogError: For errors that highlight problems that need attention.

LogException: For logging exceptions, helping to trace and handle errors that may occur during execution.

Benefits:
Optimized for Development: It provides a convenient way to log messages during development without cluttering the console in production builds.

Improved Debugging: Helps with debugging and tracking issues during development in Unity.

No Performance Impact in Production: The logging functionality is stripped out during the build process, so there’s no impact on the performance of the final game.

Overall, DevLogger is a useful tool for developers to keep track of important information during development without worrying about logging output in their shipped games.
