# logger
A project that adds color to golang's log module
# Installation
```
go get github.com/christopher18/logger
```
# Usage
```go
// Import the module
import "github.com/christopher18/logger"

// InfoLogger logger for infos
InfoLogger *logger.Logger = logger.NewFromPreset(logger.InfoType, os.Stdout)

// WarningLogger logger for warnings
WarningLogger *logger.Logger = logger.NewFromPreset(logger.WarningType, os.Stdout)

// ErrorLogger logger for errors
ErrorLogger *logger.Logger = logger.NewFromPreset(logger.ErrorType, os.Stderr)

// Use log functions as you normally would
InfoLogger.Println("Example info log")
WarningLogger.Println("Example warning log")
ErrorLogger.Println("Example error log")
```