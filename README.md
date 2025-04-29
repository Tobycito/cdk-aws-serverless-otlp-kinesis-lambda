# CDK AWS Serverless OTLP Kinesis Lambda 🚀

![GitHub Release](https://img.shields.io/github/release/Tobycito/cdk-aws-serverless-otlp-kinesis-lambda.svg?style=flat-square)
![GitHub Issues](https://img.shields.io/github/issues/Tobycito/cdk-aws-serverless-otlp-kinesis-lambda.svg?style=flat-square)
![GitHub Stars](https://img.shields.io/github/stars/Tobycito/cdk-aws-serverless-otlp-kinesis-lambda.svg?style=social)

Welcome to the **CDK AWS Serverless OTLP Kinesis Lambda** repository! This project demonstrates a serverless method to send OpenTelemetry traces to any OTel-compatible vendor using Kinesis Data Streams and AWS Lambda. 

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Overview

OpenTelemetry (OTel) provides a set of tools for observability, allowing developers to collect and export telemetry data from applications. This repository showcases how to implement a serverless architecture using AWS CDK (Cloud Development Kit) to send traces to any OTel-compatible vendor. 

With the combination of Kinesis Data Streams and AWS Lambda, this setup allows for real-time data processing and seamless integration with various telemetry backends.

## Features

- **Serverless Architecture**: Utilizes AWS Lambda and Kinesis for scalability and cost-effectiveness.
- **OpenTelemetry Support**: Easily integrates with any OTel-compatible vendor.
- **AWS CDK**: Simplifies the deployment and management of cloud resources.
- **Real-time Data Processing**: Leverages Kinesis for immediate data streaming.
- **Extensible**: Can be customized to fit various use cases.

## Architecture

![Architecture Diagram](https://example.com/path/to/architecture-diagram.png)

The architecture consists of the following components:

1. **OpenTelemetry SDK**: Instrument your application to collect traces.
2. **Kinesis Data Streams**: Acts as a buffer for incoming telemetry data.
3. **AWS Lambda**: Processes data from Kinesis and sends it to the configured OTel vendor.

## Getting Started

To get started with this project, ensure you have the following prerequisites:

- **AWS Account**: You need an AWS account to deploy the resources.
- **AWS CLI**: Install the AWS Command Line Interface to interact with AWS services.
- **Node.js**: Install Node.js, which is required for AWS CDK.
- **AWS CDK**: Install the AWS CDK globally using npm:

```bash
npm install -g aws-cdk
```

### Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/Tobycito/cdk-aws-serverless-otlp-kinesis-lambda.git
cd cdk-aws-serverless-otlp-kinesis-lambda
```

## Usage

### Configuration

Before deploying, configure the necessary environment variables:

1. Set your AWS region:

```bash
export AWS_REGION=us-west-2
```

2. Configure the OpenTelemetry endpoint:

```bash
export OTEL_ENDPOINT=https://your-otel-vendor-endpoint
```

### Running the Application

You can build and deploy the application using the following commands:

```bash
cdk synth
cdk deploy
```

This will synthesize the CloudFormation template and deploy the resources defined in the CDK stack.

## Deployment

For deployment, follow these steps:

1. Ensure your AWS credentials are configured. You can use the AWS CLI to configure them:

```bash
aws configure
```

2. Deploy the application using CDK:

```bash
cdk deploy
```

3. Monitor the deployment process in the terminal.

### Download the Latest Release

You can download the latest release from the [Releases](https://github.com/Tobycito/cdk-aws-serverless-otlp-kinesis-lambda/releases) section. Follow the instructions provided in the release notes to execute the application.

## Contributing

We welcome contributions! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Create a pull request.

Please ensure that your code adheres to the existing style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Contact

For questions or feedback, feel free to reach out:

- **GitHub**: [Tobycito](https://github.com/Tobycito)
- **Email**: toby@example.com

Thank you for your interest in the CDK AWS Serverless OTLP Kinesis Lambda project! We hope you find it useful for your observability needs. For more information, check the [Releases](https://github.com/Tobycito/cdk-aws-serverless-otlp-kinesis-lambda/releases) section for updates and new features.