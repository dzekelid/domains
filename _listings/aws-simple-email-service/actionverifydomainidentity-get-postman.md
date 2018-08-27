{
  "info": {
    "name": "AWS Simple Email Service API Verify Domain Identity",
    "_postman_id": "4afa47fd-ae02-4c81-baa6-d8d54b32256e",
    "description": "Verifies a domain.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "7b29a1de-7cfb-47cd-8ea4-f669ec2c7fea",
          "name": "cloneReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CloneReceiptRuleSet?OriginalRuleSetName=OriginalRuleSetName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule set by cloning an existing one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "617f31c9-8cb7-4e21-97ff-ac870e28f6fc"
            }
          ]
        },
        {
          "id": "0b33661d-5065-4b00-97a3-b9c6bce9fd87",
          "name": "createReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an empty receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70af9285-8ea6-4a6e-9f7b-9f9acd103aba"
            }
          ]
        },
        {
          "id": "ac1edead-53c1-429f-97a9-00a32618e21e",
          "name": "deleteReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule set and all of the receipt rules it contains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91ec9c4e-edb2-491e-a776-d6e71895c439"
            }
          ]
        },
        {
          "id": "760a99bb-79a2-4594-95f9-a5807ed27b8b",
          "name": "describeActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActiveReceiptRuleSet?Metadata=Metadata&Rules.member.N=Rules.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata and receipt rules for the receipt rule set that is currently active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d6feef9-8099-4011-bd76-93cba0726a33"
            }
          ]
        },
        {
          "id": "ac1575b5-521c-4ec3-b299-d28ef5e27d61",
          "name": "describeReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71f54c3a-71cd-4ce4-a55b-8af9f0f364ae"
            }
          ]
        },
        {
          "id": "b8d5d574-1190-4312-93f7-a04bf130d2b7",
          "name": "listReceiptRuleSets",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptRuleSets?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the receipt rule sets that exist under your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0aa6c3a-04ff-474e-8068-902c6510496a"
            }
          ]
        },
        {
          "id": "536de5fb-14c8-4bbe-afc5-f44d4fc7fb5c",
          "name": "reorderReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=ReorderReceiptRuleSet?RuleNames.member.N=RuleNames.member.N&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reorders the receipt rules within a receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6069de7e-a3f4-4912-a8f3-d0702af0b467"
            }
          ]
        },
        {
          "id": "0ef4bc27-a7dc-40fa-a0b3-d230f2e0d748",
          "name": "setActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=SetActiveReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the specified receipt rule set as the active receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2153c672-a657-4256-974b-4c21b0f3bf97"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "7c76e5b5-10bc-44b4-92ab-cfb12b7f4265",
          "name": "createConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSet?ConfigurationSet=ConfigurationSet",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4a492bd-eb19-44c9-afc5-59b76402af31"
            }
          ]
        },
        {
          "id": "7dd3aa84-2dec-4c86-a07d-cd5fcde0ef51",
          "name": "deleteConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSet?ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42bbed14-2075-4a5c-ba0c-cbd6e5699f12"
            }
          ]
        },
        {
          "id": "c538905d-a34b-48e6-b354-f751f858ec7e",
          "name": "describeConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConfigurationSet?ConfigurationSetAttributeNames.member.N=ConfigurationSetAttributeNames.member.N&ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "417dfc55-e3f9-4876-b5c2-6e53a663e92b"
            }
          ]
        },
        {
          "id": "c0d1df46-2e6a-472a-b1db-1dbb03a179f8",
          "name": "listConfigurationSets",
          "request": {
            "url": "http://example.com/api/?Action=ListConfigurationSets?MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the configuration sets associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a490251-2495-48c4-add6-a3567895b14d"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "3cba538a-fc15-41ef-a8fc-3e958f70732d",
          "name": "createConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestination=EventDestination",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "587da958-6f47-4090-ada3-d117aea43cff"
            }
          ]
        },
        {
          "id": "d1b22349-9497-4361-9801-d2535f037a56",
          "name": "deleteConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestinationName=EventDestinationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c26af5f0-334d-4e9a-b67c-40e791b04d7a"
            }
          ]
        },
        {
          "id": "1ad1c1da-a0a6-40b1-a067-b13e294cfd29",
          "name": "updateConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=UpdateConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestination=EventDestination",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the event destination of a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ad2e052-0277-4fa3-a5bb-2264bcbd79e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "f4c67578-0649-4e36-baca-b307f4426a2c",
          "name": "createReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptFilter?Filter=Filter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d63d3c7c-72a4-496a-a006-d81e5f175efe"
            }
          ]
        },
        {
          "id": "a446acdc-44aa-4c4e-b084-732773acad96",
          "name": "deleteReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptFilter?FilterName=FilterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9775506-2a68-4507-b87d-932f995b8222"
            }
          ]
        },
        {
          "id": "e3072a4a-34ab-4ddc-ae0e-f897023ee013",
          "name": "listReceiptFilters",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptFilters?Filters.member.N=Filters.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IP address filters associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "235136fa-d97c-4952-8fe2-b6194fa901aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "6847c0d8-99f9-4b68-a700-727671264e04",
          "name": "createReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRule?After=After&Rule=Rule&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1fa83cd-496a-4241-ae48-05315d4bb801"
            }
          ]
        },
        {
          "id": "5113397b-f116-49da-85d6-97bfff90a77a",
          "name": "deleteReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32bf12a4-c1f2-458c-9628-6c3b374310b8"
            }
          ]
        },
        {
          "id": "7a15fb97-e937-48a9-abc3-aba3c7fb87ed",
          "name": "describeReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48628c30-4d63-4514-b176-fba6b4ece701"
            }
          ]
        },
        {
          "id": "5f8bf5b3-c0ff-42f6-88b1-fae69c28d6e6",
          "name": "setReceiptRulePosition",
          "request": {
            "url": "http://example.com/api/?Action=SetReceiptRulePosition?After=After&RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the position of the specified receipt rule in the receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cedc08e3-194f-41bc-9b1d-f9130e2e1e31"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "8005ac04-1006-42b4-b7a4-57c3659794f2",
          "name": "deleteIdentity",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentity?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified identity (an email address or a domain) from the list of verified identities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3e4f81f-0675-4e5d-aad8-e18d07a0a7af"
            }
          ]
        },
        {
          "id": "137a4d7f-ac17-45ce-98d0-9c0365d5141d",
          "name": "deleteIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentityPolicy?Identity=Identity&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified sending authorization policy for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "065004c7-b27f-44be-9c5e-c00dc3e61760"
            }
          ]
        },
        {
          "id": "3f91c19d-11b6-4f10-8847-cc5b4db95dc8",
          "name": "getIdentityDkimAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityDkimAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current status of Easy DKIM signing for an entity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89a3d2d9-f340-4367-9863-4d00daa054fb"
            }
          ]
        },
        {
          "id": "da177bb8-7a81-4f68-90fd-ab65fc3456d7",
          "name": "getIdentityMailFromDomainAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityMailFromDomainAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the custom MAIL FROM attributes for a list of identities (email addresses and/or domains)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d862147-c85c-4a74-bf42-c41b145ec60d"
            }
          ]
        },
        {
          "id": "ada725d9-073c-4907-a8e7-40af736e8dc1",
          "name": "getIdentityNotificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityNotificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of verified identities (email addresses and/or domains), returns a structure describing identity notification attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "943d620e-eaf9-4765-87fe-ded5428ea840"
            }
          ]
        },
        {
          "id": "f262b165-933f-47df-ac7e-0432cd5c8a7f",
          "name": "getIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityPolicies?Identity=Identity&PolicyNames.member.N=PolicyNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the requested sending authorization policies for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed744be9-9f94-4c42-aeea-235bcdebf22e"
            }
          ]
        },
        {
          "id": "382ee69f-9e04-4beb-acb2-c7e4458e4cfb",
          "name": "getIdentityVerificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityVerificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of identities (email addresses and/or domains), returns the verification status and (for domain identities) the verification token for each identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "525c7a4a-3e90-4024-b2f5-aac8c49a1b20"
            }
          ]
        },
        {
          "id": "d6570d24-3914-48b8-abf5-10763ed21e3f",
          "name": "listIdentities",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentities?IdentityType=IdentityType&MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the identities (email addresses and domains) for your AWS account, regardless of verification status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8f5ebed-3fd4-4c2b-8ef6-e2993870722c"
            }
          ]
        },
        {
          "id": "550cb4fb-22b4-41fd-b19e-0e55de4ba160",
          "name": "listIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentityPolicies?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of sending authorization policies that are attached to the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50d8d7e2-0a00-4260-9659-dedb6fc00120"
            }
          ]
        },
        {
          "id": "7c2dd44d-54b3-43f6-9e91-fc213749c8c4",
          "name": "putIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutIdentityPolicy?Identity=Identity&Policy=Policy&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or updates a sending authorization policy for the specified identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ad3b6f4-e62a-40b2-b0a8-ffc17f521e1e"
            }
          ]
        },
        {
          "id": "a969d3d4-d796-4bd6-a6dc-ee91787fbd64",
          "name": "setIdentityDkimEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityDkimEnabled?DkimEnabled=DkimEnabled&Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables or disables Easy DKIM signing of email sent from an identity:If Easy DKIM\n            signing is enabled for a domain name identity (e."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b974d664-5389-4c69-af4a-49d816c9af1d"
            }
          ]
        },
        {
          "id": "471d5ee3-fa99-410f-abd2-509537c28f36",
          "name": "setIdentityFeedbackForwardingEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityFeedbackForwardingEnabled?ForwardingEnabled=ForwardingEnabled&Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), enables or disables whether Amazon SES forwards bounce and complaint notifications as email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd90ae53-e301-4980-8a29-e4e4344a476c"
            }
          ]
        },
        {
          "id": "385d4f51-c982-4e3c-9919-b7e0604dd0b2",
          "name": "setIdentityHeadersInNotificationsEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityHeadersInNotificationsEnabled?Enabled=Enabled&Identity=Identity&NotificationType=NotificationType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), sets whether Amazon SES includes \n            the original email headers in the Amazon Simple Notification Service (Amazon SNS) notifications \n            of a specified type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87af68af-73f2-4f18-bd48-992e102f5556"
            }
          ]
        },
        {
          "id": "449bb0ca-5cd9-4ac4-9ec2-12e716c6f05b",
          "name": "setIdentityMailFromDomain",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityMailFromDomain?BehaviorOnMXFailure=BehaviorOnMXFailure&Identity=Identity&MailFromDomain=MailFromDomain",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables or disables the custom MAIL FROM domain setup for a verified identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33f57930-711f-4337-8e28-a244317d9ff8"
            }
          ]
        },
        {
          "id": "53848a61-80bc-46c5-b5f9-bdbbe63bf824",
          "name": "setIdentityNotificationTopic",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityNotificationTopic?Identity=Identity&NotificationType=NotificationType&SnsTopic=SnsTopic",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), sets the Amazon Simple Notification Service (Amazon SNS) topic to which Amazon SES will publish\n        bounce, complaint, and/or delivery notifications for emails sent with that identity as the Source."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e2725dd-3479-4226-9e73-ced6c163f25b"
            }
          ]
        },
        {
          "id": "ca4f847b-4ab6-4b06-9a53-6458b6d31ecd",
          "name": "verifyDomainIdentity",
          "request": {
            "url": "http://example.com/api/?Action=VerifyDomainIdentity?Domain=Domain",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Verifies a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b95edf4d-edd2-4e41-b7d6-1f4c6caa0015"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "c17c9374-ddc4-4d69-b6c4-3e788f6e5246",
          "name": "deleteVerifiedEmailAddress",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVerifiedEmailAddress?EmailAddress=EmailAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified email address from the list of verified addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a67ff246-5ac1-436e-8962-cd2defdebacd"
            }
          ]
        },
        {
          "id": "6715797d-bfae-437d-8f31-e1c2e28ac648",
          "name": "listVerifiedEmailAddresses",
          "request": {
            "url": "http://example.com/api/?Action=ListVerifiedEmailAddresses?VerifiedEmailAddresses.member.N=VerifiedEmailAddresses.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the email addresses that have been verified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8983a53-1d72-49ef-9f9a-2f70d799814c"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Quota",
      "item": [
        {
          "id": "fd87f62f-232d-442a-a4f9-da3ba0756960",
          "name": "getSendQuota",
          "request": {
            "url": "http://example.com/api/?Action=GetSendQuota?Max24HourSend=Max24HourSend&MaxSendRate=MaxSendRate&SentLast24Hours=SentLast24Hours",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's current sending limits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cabe519-fe8a-444f-b51e-320407619b7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "1582941b-3928-4a4b-a4c4-e968b8eccffc",
          "name": "getSendStatistics",
          "request": {
            "url": "http://example.com/api/?Action=GetSendStatistics?SendDataPoints.member.N=SendDataPoints.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's sending statistics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69fec43f-52e8-4ecc-8897-4b30c40d1b12"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "7fc13c5a-c2bb-4199-bbfc-7b75f086b4e9",
          "name": "sendBounce",
          "request": {
            "url": "http://example.com/api/?Action=SendBounce?BouncedRecipientInfoList.member.N=BouncedRecipientInfoList.member.N&BounceSender=BounceSender&BounceSenderArn=BounceSenderArn&Explanation=Explanation&MessageDsn=MessageDsn&OriginalMessageId=OriginalMessageId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates and sends a bounce message to the sender of an email you received through Amazon SES."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a56adab-0aa9-4a01-8613-6d1a950edb4f"
            }
          ]
        }
      ]
    },
    {
      "name": "Email",
      "item": [
        {
          "id": "63b87510-f52c-4a17-8bc0-5be3549027a9",
          "name": "sendEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendEmail?ConfigurationSetName=ConfigurationSetName&Destination=Destination&Message=Message&ReplyToAddresses.member.N=ReplyToAddresses.member.N&ReturnPath=ReturnPath&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Composes an email message based on input data, and then immediately queues the message for sending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "791ffa04-a9af-4fd7-ab0e-30ab7592a29f"
            }
          ]
        },
        {
          "id": "508b0a01-e939-4be4-ba2b-50d22c892d59",
          "name": "sendRawEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendRawEmail?ConfigurationSetName=ConfigurationSetName&Destinations.member.N=Destinations.member.N&FromArn=FromArn&RawMessage=RawMessage&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sends an email message, with header and content specified by the client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6651056a-71ff-4267-8df3-eba96c7b3802"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rule s",
      "item": [
        {
          "id": "cd798f8f-c1d8-452f-85cb-c5d79729dec0",
          "name": "updateReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=UpdateReceiptRule?Rule=Rule&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4713d806-0626-49d2-8255-2916964840d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "35daa470-4c9c-45c0-b13e-748d1311af28",
          "name": "verifyDomainDkim",
          "request": {
            "url": "http://example.com/api/?Action=VerifyDomainDkim?Domain=Domain",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of DKIM tokens for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b26bfd26-60cf-4993-9f3b-cc1b3082e152"
            }
          ]
        }
      ]
    }
  ]
}