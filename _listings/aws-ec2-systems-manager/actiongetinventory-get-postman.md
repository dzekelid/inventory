{
  "info": {
    "name": "Amazon EC2 Systems Manager API Get Inventory",
    "_postman_id": "4ae0647b-bd40-4e3b-a379-edc2d6dee52f",
    "description": "Query inventory information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "cfcf1ac8-6c77-443e-8f0c-5f4395d63ccd",
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
              "id": "0ceca0b1-2541-4611-b170-cd947bcf0e73"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "188b84dd-2ab6-448d-b3c1-da5c6e351090",
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
              "id": "f30f1ca9-820a-47ed-b7c1-8697966f4fde"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "161d044d-17b5-4961-9c2a-457deaeb672d",
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
              "id": "401a2666-de2d-45eb-a3db-05068c11504a"
            }
          ]
        },
        {
          "id": "fa865d67-a9d9-44f9-b46e-fffdc2b94a69",
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
              "id": "34ac34f4-84bb-4a8e-b415-5ec53fa70a64"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "4318e7a2-246a-432c-b585-c8f087fdcd7d",
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
              "id": "884f51e8-eecc-40b2-9cc2-38a79c5de9d8"
            }
          ]
        },
        {
          "id": "e4ecd51d-afad-4bac-912a-862eb249f8b2",
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
              "id": "910f1403-0303-49ac-9785-3d46d2fd954c"
            }
          ]
        },
        {
          "id": "e406f6e9-9677-4212-96d1-511531e00e5f",
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
              "id": "1af444e0-cfe5-4550-99a1-14bfa2da1217"
            }
          ]
        },
        {
          "id": "6bc10b6e-f365-4279-a38c-694dfd952190",
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
              "id": "2df9f2f1-cb96-440d-8851-f9435ff0e395"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "0582fd11-3c44-4ce0-bac9-6e0beaaaf05c",
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
              "id": "adf8b61c-b6d3-441e-91b3-f686580b789f"
            }
          ]
        },
        {
          "id": "a73ca365-f4ac-49c8-a708-f9bd1e4dd3bf",
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
              "id": "4fc5160f-40d9-4a3d-8455-df0cf00653af"
            }
          ]
        },
        {
          "id": "2375326c-3630-43a0-aeed-27fbb881e37e",
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
              "id": "59cc93fe-494b-469f-877e-3df0f0ab1cc5"
            }
          ]
        },
        {
          "id": "e2ab1d3e-8f81-4144-af7d-38813ab8d12c",
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
              "id": "d290f0e0-5c1e-43a4-b853-2a1f8847124e"
            }
          ]
        },
        {
          "id": "3ca84e43-282e-4aa1-820b-9a956701b72d",
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
              "id": "05f356d7-4f2d-494b-b323-f43c356d548f"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "fb309a2a-8a89-48b5-acab-85195c0de13a",
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
              "id": "e7ee751c-0e5d-4188-abea-706c94262eb7"
            }
          ]
        },
        {
          "id": "9781d199-f6ec-473c-b524-a57a9074ec6f",
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
              "id": "9920f6b0-12b1-4c7c-b2ef-f6acd708b917"
            }
          ]
        },
        {
          "id": "8fb26a38-167a-43d0-9c57-a2c743a37478",
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
              "id": "b86ca7ca-af04-406c-b3fa-ebb1a455cefa"
            }
          ]
        },
        {
          "id": "b3bd10fc-6ea6-4ef7-83e0-5b383df88615",
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
              "id": "1f7685db-dd6b-480a-a25a-f9dfeeda89ff"
            }
          ]
        },
        {
          "id": "78e4801b-d3ec-493d-a2be-a986198e0173",
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
              "id": "4155a41a-8bf1-4e00-b88c-fff0ce4dce3a"
            }
          ]
        },
        {
          "id": "fba875cf-bfbf-4296-83ee-c32f18f957fd",
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
              "id": "5b86e333-300e-41b7-acf9-c6fd960a29ff"
            }
          ]
        },
        {
          "id": "325796f9-6d76-4e20-8b11-67669ae366f0",
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
              "id": "18eee585-169a-4164-b89b-e44fc35b21a5"
            }
          ]
        },
        {
          "id": "30902919-c871-409a-a59a-e89fb2170d91",
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
              "id": "d4317bdb-3589-4c80-b642-58d726f8186d"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "78374b0e-bc0b-40de-ac2c-d73fce33090e",
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
              "id": "0d9dfc27-8a14-467d-9268-169ecf7a5a4f"
            }
          ]
        },
        {
          "id": "61b1d5dd-b915-495a-97c9-c36423dcc762",
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
              "id": "1d5c299d-2e7a-4ead-b605-53cfca7a9a74"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "0a893fb2-6570-4918-9397-0c07f30d84bc",
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
              "id": "0b0b4965-4631-421e-97ab-7a03fe6c32ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "08b81a85-e34c-4b11-8eb9-2f6e9cea31f4",
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
              "id": "66933052-b209-4989-81a5-a47a07ee9de0"
            }
          ]
        },
        {
          "id": "60fa9fb5-fb68-4907-9b96-1e21250412e7",
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
              "id": "037edd49-f413-42e6-9eea-6358a1e6ea14"
            }
          ]
        },
        {
          "id": "bf23ae81-c146-41d7-aeff-74cc1221ba4e",
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
              "id": "2332b04d-2eed-48f8-b8f4-481ee0d1b080"
            }
          ]
        },
        {
          "id": "8ebb7b1c-7dd0-4d0c-8368-50bbfac29b4e",
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
              "id": "e517d1ce-ece4-4494-8b24-b90c0849b74e"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "d5a54dd8-5655-4509-b7f1-e6267912120e",
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
              "id": "e4f29e3b-4ae9-4fa4-bcf2-1babc0a233f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "80561726-544c-4ffe-b3c5-110210d5ec40",
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
              "id": "f6f0eeda-a759-481d-8111-3ca949114fbb"
            }
          ]
        },
        {
          "id": "7515229d-271f-436a-8365-c9ce79f7ac7a",
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
              "id": "f97a4da2-3505-483e-ac77-d93226733ba0"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "c5e000e1-3662-4d16-8140-830b6e43aa00",
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
              "id": "a8fda4d6-cfcf-4d31-b971-e41eb5b1af49"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "5ee351b8-81b6-43d2-8e59-3b3d7a6c0781",
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
              "id": "ccdfe6cc-b958-40cb-8098-782816a8da38"
            }
          ]
        },
        {
          "id": "6525ed1f-01a8-46c7-ae24-ab582b7bf29d",
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
              "id": "e117a610-7dff-4468-a749-84bff8dfd4dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "e0735286-9252-45fb-a5bf-de5f0be376c7",
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
              "id": "27eb0167-71d7-48e5-8174-e4e6482dd2b4"
            }
          ]
        },
        {
          "id": "d0f49f5b-33e3-448b-8518-ac81c6e1612c",
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
              "id": "51d9d356-a897-43eb-9426-2cfd5b52ac02"
            }
          ]
        },
        {
          "id": "8c8dea85-b308-4b04-b78e-85d585742873",
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
              "id": "96b88623-f313-4aef-a6a7-61e18fbfe56c"
            }
          ]
        },
        {
          "id": "cc021c77-d127-4750-b784-de88d9561bcd",
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
              "id": "0bc6242d-7485-4180-b2f6-7b2098e30854"
            }
          ]
        },
        {
          "id": "c1611d22-8cec-46d4-997b-e14327af5839",
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
              "id": "ed667523-0833-4fde-b1c2-635890071713"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "1f49ee49-2c9b-47ce-90c1-9067c7cf4f33",
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
              "id": "d084ab14-ab45-4ccc-95b0-0868e340e181"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "0e6e1bf1-6a71-463c-855e-699d9431f656",
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
              "id": "996b33f6-0849-4452-9de2-e27c19970b17"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "c6d37862-2edc-4f75-9900-6977df6b8473",
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
              "id": "079bb2eb-6dcf-4c50-bccf-731b13e3e483"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "c4d05ec1-f464-46ac-b4d0-d8d2e32e2df0",
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
              "id": "0995b796-e018-4d09-bad3-819a48659f34"
            }
          ]
        }
      ]
    },
    {
      "name": "Command",
      "item": [
        {
          "id": "a0daa064-6e98-4023-b1a8-90f618f76b91",
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
              "id": "85218403-4423-4964-a156-adf92d4ce7a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "c2e24511-9fe1-47ba-95ff-6c6a5ad0a6ba",
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
              "id": "6e9f77f8-32a0-40d1-bc5e-36e3d6219a11"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployable",
      "item": [
        {
          "id": "894a96e5-0977-45af-abe7-4aa3ba7b1365",
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
              "id": "fab42286-b61c-40ff-ad6c-562b163bdf1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Inventory",
      "item": [
        {
          "id": "911964f9-7e03-436c-b1db-e180eb9fdd11",
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
              "id": "e8bdf535-7c32-484c-bd37-fd4ac56b498c"
            }
          ]
        }
      ]
    }
  ]
}