<div align="center">
  <h1>Hello World Lambda</h1>
  <p>A simple AWS Lambda function written in NodeJS.</p>
</div>


## About
This repository contains code for a very simple "Hello World" AWS Lambda function written in NodeJS.

### Tech Stack
- NodeJS

## Getting Started

### Prerequisites
Ensure you have the following installed and setup
- Node JS
- AWS CLI

### Build

```
npm run zip
```

This will create a zip file named ```lambda.zip``` in the current directory.

### Deploy

You can deploy the lambda function using the AWS CLI as follows

```
aws lambda update-function-code \
  --function-name hello-world-lambda \
  --zip-file fileb://lambda.zip
```

### Test 

You can invoke the function locally as follows

```bash
aws lambda invoke --function-name hello-world-lambda output.json
cat output.json
```


## Roadmap
## Contributing

## License
Distributed under the MIT License. See LICENSE for more information.

## Acknowledgements

## Limitation of Liability
THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.