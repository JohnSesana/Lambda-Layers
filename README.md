# Lambda Layers Repository

This repository contains AWS Lambda Layers that can be reused across multiple Lambda functions. Lambda Layers allow you to manage dependencies and share code more efficiently. This guide will explain how to create, package, and deploy your own Lambda Layer.

## Table of Contents

## Table of Contents

- [What is a Lambda Layer?](#what-is-a-lambda-layer)
- [Prerequisites](#prerequisites)
- [Step-by-Step Guide](#step-by-step-guide)
  - [1. Create the Layer Structure](#1-create-the-layer-structure)
  - [2. Create Folder](#2-create-folder)
  - [3. Install Your Library and Check Files](#3-install-your-library-and-check-files)
  - [4. Zip File](#4-zip-file)
  - [5. Add Zip File to Your AWS Lambda Layers](#5-add-zip-file-to-your-aws-lambda-layers)
  - [6. Connect Your Lambda with Your Layer](#6-connect-your-lambda-with-your-layer)

## What is a Lambda Layer?

A Lambda Layer is an archive containing libraries, a custom runtime, or other dependencies that you can import into your Lambda functions. It allows you to share common code across multiple functions, reducing the package size and simplifying updates.

## Prerequisites

- **Python**: Use the same version as your lambda to avoid conflicts.
- **WSL or Linux**: To use the bash commands for the layer zip creation. Some Windows systems have problems with it.
- **ZIP utility:** The packaging process involves zipping files, so you need a tool to create ZIP archives (e.g., `zip` command on Linux/macOS, `7-Zip` on Windows).

## Step-by-Step Guide

### 1. Create the Layer Structure

Create a directory that will contain your layer code and its dependencies. The folder structure depends on the runtime of your Lambda function:

### 2. Create Folder

```bash
mkdir python
cd python
```

### 3. Install your library and check files

```bash
pip3 install pandas -t .
tree -L 1
```

### 4. Zip File

```bash
zip -r pandas_layer.zip .
```

### 5. Add zip file to your AWS Lambda Layers

`ADD PRINT HERE`

### 6. Connect your lambda with your layer

`ADD PRINT HERE`
