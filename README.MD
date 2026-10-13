# ESEP Grade Calculator



A small library that computes a student's final letter grade using weighted assignment, exam, and essay grades.

## Requirements

Go 1.24 or newer

## How to get started

1. clone the repo
2. cd esep-grade-calculator/grade-calculator

## Run all tests:
```
go test ./...
```

## Run unit tests with code coverage:
```
go test -coverprofile=coverage.txt ./...
```

## Usage

```go
gc := NewGradeCalculator()

gc.AddGrade("hw 1", 95, Assignment)
gc.AddGrade("midterm", 88, Exam)
gc.AddGrade("ethics essay", 91, Essay)

letter := gc.GetFinalGrade()
```

Types of Grades: Assignemnt, Exam, Essay

