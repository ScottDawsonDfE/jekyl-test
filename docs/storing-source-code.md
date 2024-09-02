layout: page
title: "Storing source code"
permalink: /storing-source-code

# Storing Source Code
All of our source code should be open by standard, and stored on a well known and supported hosting service.

## Description
This standard applies to all new code produced within the department. Existing code should be stored to also meet
this standard but may need remediation to make this possible.

All new code produced by the department should be stored on publicly accessible repositories and have an open licence
applied in line with [point 3 of the GDS technology code of practice](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice). This standard is partially based upon the 
guidance [When code should be open or closed](https://www.gov.uk/government/publications/open-source-guidance/when-code-should-be-open-or-closed).

In addition to storing code in publicly accessible repositories, the code should be licensed using an appropriate open 
source licences to enable others to make use of the source code and to allow contributions from people outside the 
department.

## Rationale
Making source code publicly available and open source allows for other people including those in other government 
departments and outside of government to:
- benefit from your work and build upon it
- learn from your experiences
- find uses for your code which you have not found or implemented

Meeting this standard also ensures that people working within the department can easily gain access to source code from 
a central place reducing the time to onboard a person onto a project.

## Approved delivery
- The repository must be on GitHub, within the [DfE Digital organisation](https://github.com/DFE-Digital).
- The repository must be public.
- At the root level of the repository there must be a licence file name LICENCE, where the first listed licence is the 
MIT licence. Using the [MIT licence template from the open source initiative](https://opensource.org/license/MIT).
  - The copyright holder for the template is "Crown Copyright (Department for Education)".
  - Any additional licences that apply must also be recorded in the licence file.

## Tolerated delivery
For existing code, numerous changes may be needed to make the code suitable for being public and open source. If the 
code is not being actively worked on, it can remain where it is.

When existing code is actively worked on, a clear plan needs to be made for making the source code meet the same 
standard as new code. At this point an exception should be logged highlighting the plan for migration to the approved 
delivery.

## Known Exceptions
### Existing licences
For existing code, which is already licenced with an alternate licence that is not compatible with the MIT licence, 
the LICENCE file can make clear the alternate licence agreement and copyright notice.

### Code that must remain internal or closed source
Some code can remain closed source and should be held within private repositories, covered in the following 
subsections. These items should still be located within the [DfE Digital organisation](https://github.com/DFE-Digital), but can sit within a 
private repository. The following are acceptable reasons for not making code open source.

#### Keys and credentials
You must keep secret data such as keys or credentials closed, as this information could allow someone to gain access 
to your system.

You must keep code that uses secrets away from the secrets themselves. This includes storing secret keys and 
credentials separately. You can then open the code while keeping the secrets closed and secure.

For example, you can use a secret management system to store and secure your secrets, but allow applications to use 
them where necessary. A secret management system makes sure the keys can only be accessed by authorised staff. 
The system also makes it easier to provide different keys for different environments and rotate keys if needed.

#### Unreleased policy
If the code makes clear details of a policy that has not yet been announced, 
you should keep the code closed until the policy is announced.

However, you must develop the code as if it’s already open, and you must open the code as soon as 
possible after the policy is announced.

#### Fraud detection algorithms
You should close any algorithms you use to detect fraud. You should also separate any code using them from the 
algorithms themselves. The separation will make it easier for you to update the algorithms as you learn more about 
the attempts to defraud your system.

## Document control
| Version   | Date       | Comments                                                          |
|-----------|------------|-------------------------------------------------------------------|
| 0.1 Draft | 2024-06-13 | Updated to include sections similar to the DDT standards document |
| 0.2 Draft | 2024-08-08 | Grammar corrections                                               |
