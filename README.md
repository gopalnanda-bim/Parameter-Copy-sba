## Parameter Copy – SDA

**pyRevit extension for copying shared parameter values across multiple elements in Revit models.**


## Who is this for?

This extension is designed for:

- Electrical planners (Elektroplaner)
- BIM modellers working in TGA projects
- Engineers working with mixed families and categories in Revit

---

## Background: Parameter Management in Revit

In real-world BIM projects, parameter data is often:

- distributed across multiple families  
- inconsistent between elements  
- difficult to standardize at scale  

Manually copying parameter values between elements can be:

- time-consuming  
- error-prone  
- unreliable when working across categories  

Standard Revit workflows do not provide a safe and efficient way to copy parameters across multiple elements with validation.

---

## What this tool does

This tool allows users to copy parameter values from a single source element to multiple target elements, even across different families or categories.

Unlike generic parameter copy tools, it:

- automatically detects parameters shared across all selected elements  
- prevents invalid parameter assignments  
- ensures safe and consistent data transfer  

---

## Features

### Source → Multi-Target Workflow

- Select one source element  
- Select multiple target elements  
- Use toggle-based selection for flexibility  

---

### Smart Parameter Filtering

- Displays only common parameters (intersection across all elements)  
- Eliminates invalid or missing parameter options  
- Reduces user error significantly  

---

### Supported Parameter Types

- String  
- Integer  
- Double  
- ElementId  

---

### Safe Execution

- Skips:
  - read-only parameters  
  - missing parameters  
  - incompatible parameter types  
- Prevents crashes and incorrect assignments  

---

### Execution Summary

- Provides a clear report after execution  
- Confirms:
  - which parameters were copied  
  - how many elements were updated  

---

## Typical Use Cases

- Copying installation height or metadata across devices  
- Synchronizing MEP room-related information  
- Standardizing shared parameters across different families  
- Cleaning and aligning BIM data in mixed-category models  

---

## Why this matters in practice

In BIM workflows, data consistency is as critical as geometry.

This tool enables:

- fast and reliable parameter standardization  
- reduced manual editing effort  
- fewer data inconsistencies in project models  

It is especially useful in large projects where elements come from multiple families and sources.

---

## Requirements

- Autodesk Revit 2020 or newer  
- pyRevit (IronPython)  

---

## Installation

1. Install pyRevit  
   https://docs.pyrevitlabs.io/  

2. Clone this repository into:

   %APPDATA%\pyRevit\Extensions

3. Restart Revit  

---

## Roadmap (planned)

- Parameter presets for frequently used workflows  
- Persistent user settings  
- Extended support for additional parameter types  
- Improved UI for large element selections  
