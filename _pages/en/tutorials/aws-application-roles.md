---
title: AWS - Application / IAM Roles
#altLangPrefix: aws-???
description: All about AWS IAM Roles
tags: [aws, tutorial, iam, boundary-policy]
draft: true
last_updated: 2025-11-28T21:49:56Z
---

Our clients are allowed to create custom application roles / IAM roles, but to prevent privilege escalation, a permission boundary called `SSCCustomRoleBoundaryPolicy` is required.  The combination of Permission Boundaries and Service Control Policies is an advanced feature that limits the maximum permissions that a role can grant to an IAM entity. An entity's permissions boundary allows it to perform only the actions that are allowed by both its identity-based policies and its permissions boundaries.  

In almost all cases, when creating a new application role or IAM role in AWS you will need to attach a boundary policy. These policies are maintained by the CIE (LaunchPad) Operations team. 

> Note that in the past we used a policy called `SSCDeveloperBoundaryPolicy`  (and `SSCPowerUserBoundaryPolicy`); although you might see this role in some places, it can not be used for any new roles. Fortunately `SSCCustomRoleBoundaryPolicy` is a drop-in replacement for `SSCDeveloperBoundaryPolicy`.
{.is-warning}


The two main  boundary policies that are provisioned to our accounts are `SSCCustomRoleBoundaryPolicy` and `SSCPowerUserBoundaryPolicy`.

-   `SSCPowerSysadminBoundaryPolicy` is applied to user accounts for actual users, to set appropriate policies for the PowerSysadmin role. This policy can not be used for custom roles.
-   `SSCCustomRoleBoundaryPolicy` is the policy that must be set on custom IAM roles.

If using the web portal to create a new IAM role, you can attach the boundary policy using the 'Set permissions boundary - *optional*' box, clicking the 'Use a permissions boundary \[...\]' option, searching for 'ssc', and finally select the Custom Role policy:

![](/assets/images/aws_webui_set_permissions_boundary_new_role.png)

LaunchPad team members can find operational details about our Boundary Policies on the [AWS - Boundary Policies](/en/tutorials/aws-boundary-policies) page.
