This section contains requirements for the system.

## Requirements Overview

{{
  
List and link to the high-level requirements of the system.
You may also list and link to the most impactful 10 to 20 requirements of the system.

}}

## Requirements Workflow

The folder structure reflects the intended workflow on how requirements should be handled.

1. Requirements are **proposed**, and moved into the `5.v-REQprop` folder
2. Once a requirement has enough information available to be implemented, it is **ready**, and should be moved to the `5.w-REQrdy` folder
3. A requirement in **proposed** or **ready** state may be **declined**, meaning that it will not be implemented, and must be moved to the `5.z-REQdecl` folder
4. When the implementation of a requirement is merged into the *main* branch, the requirement gets **active**, and must be moved to the `5.a-REQact` folder
5. If a requirement is replaced or removed by another requirement, the requirement gets **deprecated**, and must be moved to the `5.y-REQdepr` folder 

   **Note:** A link must be added to the **deprecated** requirement, pointing to the new requirement.

## Requirements Tag

Tags help to easily reference requirements.
Requirement tags may be grouped to create a hierarchy of requirements.

**Note:** Tags must not include any whitespace or `-` to keep tags readable in wiki titles.