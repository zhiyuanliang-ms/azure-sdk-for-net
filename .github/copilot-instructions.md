# Project Overview

This repo contains Azure SDKs for various Azure services and tools that generate them.

## Prerequisites
- To use MCP tool calls, PowerShell must be installed. Provide [PowerShell installation instructions](https://learn.microsoft.com/powershell/scripting/install/installing-powershell) if not installed, and recommend restarting the IDE to use the MCP server.

## Folder Structure

- `/eng/packages/http-client-csharp`: Contains the source code of the generator for Azure Data Plane SDKs (aka Azure Generator).
- `/eng/packages/http-client-csharp-mgmt`: Contains the source code of the generator for Azure Management Plane SDKs (aka Azure Management Generator).
- `/sdk`: Contains the individual SDKs for Azure services.

### Azure Generator

- Always run `npm install` in the `/eng/packages/http-client-csharp` directory before running the generator.
- Always run `/eng/packages/http-client-csharp/eng/scripts/Generate.ps1` to regenerate the test projects to validate the result of generator code changes.

### Azure Management Generator

- Always run `npm install` in the `/eng/packages/http-client-csharp-mgmt` directory before running the generator.
- Always run `/eng/packages/http-client-csharp-mgmt/eng/scripts/Generate.ps1` to regenerate the test projects to validate the result of generator code changes.

## SDK release

For detailed workflow instructions, see [SDK Release](https://github.com/Azure/azure-sdk-for-net/tree/main/eng/common/instructions/copilot/sdk-release.instructions.md).