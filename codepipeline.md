## CodePipeline

- ##  工作流程建模

  管道定义了您的发布工作流程，并描述了新代码更改在发布过程中的进展情况。管道包括一系列阶段（例如，构建、测试和部署），可充当您工作流程中的逻辑分区。每个阶段由一系列操作组成，如构建代码或部署到测试环境等任务。AWS  CodePipeline  为您提供了一个图形用户界面，用于创建，配置和管理您的管道及其各个阶段和操作，使您可以轻松地对发布工作流程进行可视化和建模。

  **并行执行**
   您可以使用 CodePipeline 对构建、测试和部署操作进行建模，以便并行运行，从而提高工作流程的速度。

- ##  AWS integrations

  AWS CodePipeline 可以直接从 [AWS CodeCommit](https://aws.amazon.com/cn/codecommit/)、[GitHub](https://docs.aws.amazon.com/codepipeline/latest/userguide/pipelines-webhooks-migration.html)、[Amazon ECR](https://aws.amazon.com/cn/ecr/) 或 [Amazon S3](https://aws.amazon.com/cn/s3/) 为您的管道提取源代码。它可在 [AWS CodeBuild](https://aws.amazon.com/cn/codebuild/) 中运行构建和单元测试。CodePipeline 可使用 [ AWS CodeDeploy](https://aws.amazon.com/cn/codedeploy/)、[AWS Elastic Beanstalk](https://aws.amazon.com/cn/elasticbeanstalk/)、[Amazon Elastic Container Service](https://aws.amazon.com/cn/ecs/) (Amazon ECS) 或 [AWS Fargate](https://aws.amazon.com/cn/fargate/) 部署您的更改。

  您还可以对 [AWS CloudFormation](https://aws.amazon.com/cn/cloudformation/) 操作进行建模，从而在发布流程中预置、更新或删除 AWS 资源。如此一来，您还能持续交付使用 [AWS Lambda](https://aws.amazon.com/cn/lambda/)、[Amazon API Gateway](https://aws.amazon.com/cn/api-gateway/)、[Amazon DynamoDB](https://aws.amazon.com/cn/dynamodb/) 和 [AWS Serverless Application Model](https://github.com/awslabs/serverless-application-model) (AWS SAM) 构建的无服务器应用程序。

  您也可以使用 CodePipeline [与 AWS Lambda 的集成](http://docs.aws.amazon.com/codepipeline/latest/userguide/how-to-lambda-integration.html)，在管道的任意阶段触发由代码定义的自定义函数。例如，您可以触发一个测试您的 Web 应用程序是否成功部署的 Lambda 函数。

  借助 CodePipeline，您可以配置一个将这些服务与[第三方开发人员工具](https://aws.amazon.com/cn/codepipeline/product-integrations/)和自定义系统联系在一起的管道。

- AWS code commit; -- > codedeploy -> codePipeline -> 测试；
- 
- [AWS preparedness](https://medium.com/@bachlmayr/how-to-master-the-aws-devops-professional-exam-de2b80ae10e2)