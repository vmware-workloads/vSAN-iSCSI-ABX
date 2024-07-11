# vSAN-iSCSI-ABX

This is an ABX extension for Aria Automation to create iSCSI targets/LUNS.

## Install

### Action Constants

We start by adding the Ansible Automation Platform URL and credentials that will be used by the actions. 

1. Under  **Extensibility**, then **Actions Constants**.
   <br>
   <br>
   <img src="./assets/images/action_constants.png" alt="AAP Actions" width="400"/>


2. Add the following parameters:
   * ***VC_user**: vCenter Username
   * ***VC_password***: vCenter Password
   * ***VC_url***: vCenter URL

### Actions

Add the create / read / delete actions into Aria Automation:

1. In Aria Automation Assembler, open **Extensibility**, then select **Actions**.

2. Create new actions for the 'create', 'read' and 'destroy' ABX

3. In the **Default Inputs** section, create three defaults corresponding to the action constants created previously

   * 'Action Type' should be 'Action Constant'
   * Name should be the same name as the action constant (e.g. VC_user)
   * In the drop-down, select the appropriate value mapping

   
