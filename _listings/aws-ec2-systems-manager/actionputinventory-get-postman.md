{
  "info": {
    "name": "Amazon EC2 Systems Manager API Put Inventory",
    "_postman_id": "218ca574-2189-41a7-9c69-aa7eccc52ab5",
    "description": "Bulk update custom inventory items on one more instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "4a6cc21d-b305-47c7-b70a-eb0bb862c9fc",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&ResourceType=ResourceType&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46613a2d-d76a-414c-a1eb-906fe1a410de"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "cca4bb39-c89f-489c-a0c8-c31b653f5540",
          "name": "cancelCommand",
          "request": {
            "url": "http://example.com/api/?Action=CancelCommand?CommandId=CommandId&InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to cancel the command specified by the Command ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a53f3c6-3182-4e82-af75-f3a7cc16abd9"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "a9195b3d-8098-418c-b36d-73ab08760ba3",
          "name": "createActivation",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivation?DefaultInstanceName=DefaultInstanceName&Description=Description&ExpirationDate=ExpirationDate&IamRole=IamRole&RegistrationLimit=RegistrationLimit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage\n   these resources using Run Command."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2235050f-3903-475c-a63d-c08c165461a1"
            }
          ]
        },
        {
          "id": "b9c316b6-30a1-4095-b96e-91654c7d3b16",
          "name": "deleteActivation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivation?ActivationId=ActivationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b15f47c8-58c0-4e17-8cce-fa6904feb0fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "cc263512-9b92-43a6-9c48-f39444f6fbb5",
          "name": "createAssociation",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociation?DocumentVersion=DocumentVersion&InstanceId=InstanceId&Name=Name&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression&Targets=Targets",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94ac6841-5c0a-4139-b55e-100176b2e8f9"
            }
          ]
        },
        {
          "id": "b66d9569-0f35-4877-8cc4-99a857966e1d",
          "name": "createAssociationBatch",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociationBatch?Entries=Entries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cdb14290-62f2-4e30-95ab-0199bed1ad4b"
            }
          ]
        },
        {
          "id": "7c9c80b7-e5bc-4107-9455-2a0e6c61aaa8",
          "name": "deleteAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified SSM document from the specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62640dbd-9a55-499a-8ba8-d0fb9f2bbc73"
            }
          ]
        },
        {
          "id": "2b662ad1-8b87-43f5-bb8e-575063d2c773",
          "name": "describeAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73ab7498-3d70-4e6d-aaa5-0c852bfa288f"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "67872a5a-21bf-4f85-9c97-9b5117d64e56",
          "name": "createDocument",
          "request": {
            "url": "http://example.com/api/?Action=CreateDocument?Content=Content&DocumentType=DocumentType&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ebb6dea-5386-4ee7-919e-0a841cbaf71f"
            }
          ]
        },
        {
          "id": "aff76b09-ba34-4a45-b280-c53d9f53b93d",
          "name": "deleteDocument",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDocument?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the SSM document and all instance associations to the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae3c9ead-418e-4b89-90ea-f8c783532ffd"
            }
          ]
        },
        {
          "id": "7639550a-a33e-46c5-b1f9-53de6d4623a8",
          "name": "describeDocument",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "680fe4b5-2257-49f7-9401-8dd351e480a0"
            }
          ]
        },
        {
          "id": "0f2ca581-81dd-4744-8d10-a8f863fa03ae",
          "name": "describeDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocumentPermission?Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f7ba10c-e411-4393-8116-41a119b8ea03"
            }
          ]
        },
        {
          "id": "138a2fdf-0bd2-48ba-868a-ba526a2cab07",
          "name": "getDocument",
          "request": {
            "url": "http://example.com/api/?Action=GetDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the contents of the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cd93416-db6f-42c6-97fb-5a321f813a34"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "22ca09ca-11f9-4f8b-96ad-98075ace0edf",
          "name": "createMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=CreateMaintenanceWindow?AllowUnassociatedTargets=AllowUnassociatedTargets&ClientToken=ClientToken&Cutoff=Cutoff&Duration=Duration&Name=Name&Schedule=Schedule",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdbaefeb-df89-42da-ac0b-f44bae193079"
            }
          ]
        },
        {
          "id": "a62bae82-9c34-4c82-8da4-cba35aadd76b",
          "name": "deleteMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeleteMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c91097e1-84a6-4581-b382-49b8246ec805"
            }
          ]
        },
        {
          "id": "73f3253b-55a2-438a-a54a-7b0e332a5800",
          "name": "describeMaintenanceWindowExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the executions of a Maintenance Window (meaning, information about when the\n   Maintenance Window was scheduled to be active and information about tasks registered and run with\n   the Maintenance Window)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3d93dab-ae02-4681-8233-4fb31c16c18e"
            }
          ]
        },
        {
          "id": "875003cc-d5a3-474f-85cd-ff538c1debd9",
          "name": "describeMaintenanceWindowExecutionTaskInvocations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTaskInvocations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the individual task executions (one per target) for a particular task executed\n   as part of a Maintenance Window execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d562c874-69c5-4881-814b-2b04dc72db6c"
            }
          ]
        },
        {
          "id": "7a96223a-93b8-41b2-aa68-14cce5b4ef8c",
          "name": "describeMaintenanceWindowExecutionTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a given Maintenance Window execution, lists the tasks that were executed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cb428b3-3509-4c49-ae7b-eb49f989a11e"
            }
          ]
        },
        {
          "id": "c726a80b-5518-4bc7-9149-058f35698729",
          "name": "describeMaintenanceWindows",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindows?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the Maintenance Windows in an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3de4d6fe-2b88-4b2d-a140-39703ddfe8d3"
            }
          ]
        },
        {
          "id": "22b1f60b-d7ba-484b-be2d-cc2a1a598dd9",
          "name": "describeMaintenanceWindowTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTargets?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the targets registered with the Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "936d9ee1-3fbf-48c0-8f19-b87791057317"
            }
          ]
        },
        {
          "id": "ec419efe-6823-49bc-a183-adde34cc9f02",
          "name": "describeMaintenanceWindowTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the tasks in a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dea96027-2095-43ce-b91d-e2b1b14ceeec"
            }
          ]
        },
        {
          "id": "8065b2c0-10f4-4753-b360-8f728e57c1d9",
          "name": "getMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e74cda9-6a4a-436d-ade0-eeafbe1a36c1"
            }
          ]
        },
        {
          "id": "e27ab909-3947-4fc0-a14a-bcbd260245b9",
          "name": "getMaintenanceWindowExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindowExecution?WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves details about a specific task executed as part of a Maintenance Window\n   execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "904f01ae-7127-494f-a8aa-b4b65a06c59c"
            }
          ]
        },
        {
          "id": "132eed8d-78f2-4c31-a28a-142014861b13",
          "name": "getMaintenanceWindowExecutionTask",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindowExecutionTask?TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details about a specific task executed as part of a Maintenance Window\n   execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2cf68f4-ff93-4376-b9cf-e27324cb5c02"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "1c0735c0-6f07-4d9c-9f0e-4eab757bb8d1",
          "name": "createPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePatchBaseline?ApprovalRules=ApprovalRules&ApprovedPatches=ApprovedPatches&ClientToken=ClientToken&Description=Description&GlobalFilters=GlobalFilters&Name=Name&RejectedPatches=RejectedPatches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66483797-cc9c-4a3c-8f68-f780e66cf362"
            }
          ]
        },
        {
          "id": "d2f74972-f2fd-4f41-869b-058aa6e3fbc8",
          "name": "deletePatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89cbec76-9503-4352-89c6-a96cdb883ad5"
            }
          ]
        },
        {
          "id": "f04dff10-fe8e-4cd2-974d-118df3efe9db",
          "name": "getPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7ee16bd-808a-4600-aaf1-64d33ac88c7c"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "db5eff41-1f2e-4e00-863f-4d72e8a82a84",
          "name": "deleteParameter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteParameter?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a parameter from the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f25e0309-3385-407c-b458-33ea571dcfc9"
            }
          ]
        },
        {
          "id": "2c154c53-9261-4332-81d1-d9c97bc6adf3",
          "name": "getParameterHistory",
          "request": {
            "url": "http://example.com/api/?Action=GetParameterHistory?MaxResults=MaxResults&Name=Name&NextToken=NextToken&WithDecryption=WithDecryption",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query a list of all parameters used by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d1c9d83-1969-46d1-8ce5-08c392f9a8a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "b8eec606-d006-4882-b605-52a2dbb34ee7",
          "name": "deregisterManagedInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterManagedInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the server or virtual machine from the list of registered servers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "809986ba-860c-452c-8e92-a33ed54297f7"
            }
          ]
        },
        {
          "id": "4b052e9e-3ab0-452f-83d4-f6542400a21a",
          "name": "deregisterPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a patch group from a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3263660-9391-4194-8c90-4c1871137f6d"
            }
          ]
        },
        {
          "id": "9ffb3a5b-3907-4eb4-a504-3fbaac2a6ab0",
          "name": "deregisterTargetFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargetFromMaintenanceWindow?WindowId=WindowId&WindowTargetId=WindowTargetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a target from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2937eee2-5c5e-413e-bb35-621bdf18632c"
            }
          ]
        },
        {
          "id": "7893d947-8012-477e-b2d7-bf32cd336bb8",
          "name": "deregisterTaskFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskFromMaintenanceWindow?WindowId=WindowId&WindowTaskId=WindowTaskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a task from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d1c8ce4-6143-4ddc-b07e-0d8355e9830a"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "2059f19d-b739-4149-8e83-178d209e765a",
          "name": "describeActivations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about the activation, including: the date and time the activation was created,\n   the expiration date, the IAM role assigned to the instances in the activation, and the number of\n   instances activated by this registration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "861a96d1-c860-4fbf-899b-8ad79db41682"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "b14cee34-4644-4933-b105-8aa4eeab1c12",
          "name": "describeAutomationExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutomationExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides details about all active and terminated Automation executions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d983555c-6d3e-40e2-963b-b3ae41a3bbad"
            }
          ]
        },
        {
          "id": "bb893dd1-c5b7-4064-8920-554335c4c841",
          "name": "getAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetAutomationExecution?AutomationExecutionId=AutomationExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get detailed information about a particular Automation execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b6d0698-e280-4e1f-82fb-d882ef2abca7"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "820d749e-f828-4ffb-8c5a-4426c31d8abe",
          "name": "describeAvailablePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailablePatches?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patches that could possibly be included in a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e298df6c-ea0c-4d76-8067-ef91d82e6cbf"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "8e0823c3-c6b3-4576-a56f-f39e5bfe3235",
          "name": "describeEffectiveInstanceAssociations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectiveInstanceAssociations?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e2c1d90-16b9-4fd1-8aed-6e9fc89b054a"
            }
          ]
        },
        {
          "id": "dfd6c2ab-f08d-400b-85f9-b6ad15f48834",
          "name": "describeEffectivePatchesForPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectivePatchesForPatchBaseline?BaselineId=BaselineId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current effective patches (the patch and the approval state) for the specified patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "320bde45-7fa0-49bf-ad42-5854f0dcaaa6"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "e94166f8-654f-48b9-ad80-0584c53c623d",
          "name": "describeInstanceAssociationsStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceAssociationsStatus?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The status of the associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29563fea-e00c-4aad-a895-67f6e7f4d0a3"
            }
          ]
        },
        {
          "id": "ff29bf88-e014-42a1-a5f8-1fac67bed2ed",
          "name": "describeInstanceInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceInformation?Filters=Filters&InstanceInformationFilterList=InstanceInformationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1938814c-7508-4261-a100-8b903b56b89a"
            }
          ]
        },
        {
          "id": "42307c60-084a-433e-9bd1-6036f5c22251",
          "name": "describeInstancePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatches?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the patches on the specified instance and their state relative to the patch baseline being used for the instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "146f447b-4835-4a95-9cf8-9e923ae63bc7"
            }
          ]
        },
        {
          "id": "491da069-0a3c-495b-903e-d99dcc808d3b",
          "name": "describeInstancePatchStates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStates?InstanceIds=InstanceIds&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state of one or more instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a105b33-230c-4316-a1cf-400f9f044c50"
            }
          ]
        },
        {
          "id": "b92f7ff5-2521-4a5d-bbc5-5a22e0990743",
          "name": "describeInstancePatchStatesForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStatesForPatchGroup?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state for the instances in the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "628f838b-85cf-423b-904a-bc4ba9720a2c"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "7bbef104-5860-4860-90ef-55adcf915bc4",
          "name": "describeParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeParameters?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d185a88-f81b-4f09-a48c-0442e907e3a0"
            }
          ]
        },
        {
          "id": "0ae4de65-66eb-4126-8307-4bb46993d450",
          "name": "getParameters",
          "request": {
            "url": "http://example.com/api/?Action=GetParameters?Names=Names&WithDecryption=WithDecryption",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of parameters used by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e928530-f767-48dc-b136-0cd0b5ca64be"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "48547381-609c-4593-8d5f-64e569d37364",
          "name": "describePatchBaselines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchBaselines?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the patch baselines in your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d492f93-a0a3-440f-80f7-39b69190a1a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "da83b93f-f454-4545-9549-7dd40993c04a",
          "name": "describePatchGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroups?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patch groups that have been registered with patch baselines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba422cb9-a07d-4519-9aa6-ad4bf27ea9cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "b0f14d29-59d1-4990-967d-33f9bd60a362",
          "name": "describePatchGroupState",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroupState?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns high-level aggregated patch compliance state for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "934b629c-3867-412a-b270-89801af57811"
            }
          ]
        }
      ]
    },
    {
      "name": "Command",
      "item": [
        {
          "id": "7c9527f2-b549-4cff-863a-a81fa9bb8fd8",
          "name": "getCommandInvocation",
          "request": {
            "url": "http://example.com/api/?Action=GetCommandInvocation?CommandId=CommandId&InstanceId=InstanceId&PluginName=PluginName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information about command execution for an invocation or plugin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca25ceb1-5e14-4b25-85a0-684cfeb7de5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "4c83f168-68ea-4540-95e5-f6240fe4b54b",
          "name": "getDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3394600-144b-420a-8359-ce68b4923350"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployable",
      "item": [
        {
          "id": "c2c0153e-34da-4b6a-9ca2-662ed60eff71",
          "name": "getDeployablePatchSnapshotForInstance",
          "request": {
            "url": "http://example.com/api/?Action=GetDeployablePatchSnapshotForInstance?InstanceId=InstanceId&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current snapshot for the patch baseline the instance uses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e573e7a-3cf0-4dbf-9bdc-a35119b7c42c"
            }
          ]
        }
      ]
    },
    {
      "name": "Inventory",
      "item": [
        {
          "id": "0ff788d5-16f5-43ba-8d31-55c593482b8a",
          "name": "getInventory",
          "request": {
            "url": "http://example.com/api/?Action=GetInventory?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&ResultAttributes=ResultAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query inventory information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bdd336b-d121-44da-b5a8-d23c9d006b54"
            }
          ]
        },
        {
          "id": "61e37ed2-afb8-4860-a887-b6a1970dd518",
          "name": "getInventorySchema",
          "request": {
            "url": "http://example.com/api/?Action=GetInventorySchema?MaxResults=MaxResults&NextToken=NextToken&TypeName=TypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of inventory type names for the account, or return a list of attribute\n   names for a specific Inventory item type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49e3ba23-f210-4867-9fbe-52238cd981b0"
            }
          ]
        },
        {
          "id": "31b45811-3053-45c4-a653-32ae2fad7f19",
          "name": "putInventory",
          "request": {
            "url": "http://example.com/api/?Action=PutInventory?InstanceId=InstanceId&Items=Items",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Bulk update custom inventory items on one more instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de544fa3-89f9-47e6-8729-b358a99d9c8a"
            }
          ]
        }
      ]
    },
    {
      "name": "BaselineGroup",
      "item": [
        {
          "id": "a4cf1564-9046-4bb0-b966-7facf048de91",
          "name": "getPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=GetPatchBaselineForPatchGroup?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the patch baseline that should be used for the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5563b87d-824a-4ea6-b01f-072e3b674ab1"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "85e47b46-9ea0-45e2-ac60-71ff428199cb",
          "name": "listAssociations",
          "request": {
            "url": "http://example.com/api/?Action=ListAssociations?AssociationFilterList=AssociationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b2f8d81-78fe-451f-9ec7-d1487051dc59"
            }
          ]
        },
        {
          "id": "527bae11-0c17-4f16-9d71-b7c2f1e3b5a3",
          "name": "listCommandInvocations",
          "request": {
            "url": "http://example.com/api/?Action=ListCommandInvocations?CommandId=CommandId&Details=Details&Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An invocation is copy of a command sent to a specific instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30c59892-2bfe-41e6-a697-c5b4169c632e"
            }
          ]
        },
        {
          "id": "c8225664-79df-4ae0-90e9-e39741e44c77",
          "name": "listCommands",
          "request": {
            "url": "http://example.com/api/?Action=ListCommands?CommandId=CommandId&Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the commands requested by users of the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fdb8766-6eaa-4576-a6b6-ef01a783b744"
            }
          ]
        },
        {
          "id": "2626f86c-3e1b-4f83-af50-61f1696ea51c",
          "name": "listDocuments",
          "request": {
            "url": "http://example.com/api/?Action=ListDocuments?DocumentFilterList=DocumentFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your SSM documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "462766bb-2730-4d49-a448-3e85bc04a2a0"
            }
          ]
        },
        {
          "id": "dd0f354c-72e5-4bed-b3ef-21c2aff55587",
          "name": "listDocumentVersions",
          "request": {
            "url": "http://example.com/api/?Action=ListDocumentVersions?MaxResults=MaxResults&Name=Name&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all versions for a document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7c9f04e-e81e-437f-bb56-6746088e4d4b"
            }
          ]
        },
        {
          "id": "aecade29-687d-4a46-b31e-394b720d0d13",
          "name": "listInventoryEntries",
          "request": {
            "url": "http://example.com/api/?Action=ListInventoryEntries?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken&TypeName=TypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of inventory items returned by the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a8a0705-093b-4382-9903-bfd87dc29826"
            }
          ]
        },
        {
          "id": "1a91bf47-e029-4143-9d71-257cacacc14b",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?ResourceId=ResourceId&ResourceType=ResourceType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the tags assigned to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "560630af-228e-4d37-a24a-14e3eb0c4072"
            }
          ]
        }
      ]
    },
    {
      "name": "Modify",
      "item": [
        {
          "id": "3e5dca55-e877-49d7-b2c4-123aedaed5b5",
          "name": "modifyDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDocumentPermission?AccountIdsToAdd=AccountIdsToAdd&AccountIdsToRemove=AccountIdsToRemove&Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Share a document publicly or privately."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04494a24-b1bc-4cd3-933a-3d73674b44bb"
            }
          ]
        }
      ]
    }
  ]
}