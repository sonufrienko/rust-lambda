# Build and deploy AWS Lambda function with Rust

## Getting started

1. Install [Cargo Lmabda](https://www.cargo-lambda.info/guide/getting-started.html)
2. cargo lambda new conversations
   > Is this function an HTTP function? **Yes**
   > Which service is this function receiving events from? **AWS Lambda function URLs**
3. change metadata in **Cargo.toml** file

## How to test it locally

1. cd conversations
2. cargo lambda watch
3. open http://localhost:9000/?name=Sergii

## How to deploy

1. cd conversations
2. cargo lambda build --release
3. cargo lambda deploy --region=eu-west-1
