# asyncapi-avro-shared-model
Example of a little AsyncApi file that uses Avro. 
It is here to show a problem with some [AsyncApi plugins/generator](https://github.com/asyncapi/generator/).

The problem comes from the fact that both `User` and `Pet` use the same shared `Address` model.

See issue https://github.com/asyncapi/generator/issues/1075

## To reproduce the issue

Run `generate-correct.sh` to verify that the generation works correctly. 

Run `generate-wrong.sh` to see that the generator sends `Generator Error: Input is not a correct AsyncAPI document so it cannot be processed.`
