*************************************************

1- npx create-near-app todo

2- yarn install

3- yarn dev

4- yarn build:release

5- near dev-deploy 


or run ./scripts/build.sh instead of 4,5



*************************************************

near view dev-1645348898006-52720569179472 hello

near call dev-1645348898006-52720569179472 greetingUser --account_id tilek.testnet 

near call dev-1645348898006-52720569179472 showMyQuestions --account_id tilek.testnet
near call dev-1645348898006-52720569179472 showMyAnswers --account_id tilek.testnet 

near call dev-1645348898006-52720569179472 addQuestion '{"question":"What is a sharding?"}' --account_id tilek.testnet
near call dev-1645348898006-52720569179472 addQuestion '{"question":"What is WEB 3?"}' --account_id tilek.testnet
near call dev-1645348898006-52720569179472 addAnswer '{"answer":"Sharding does a horizontal partition of your database and turns into smaller, more manageable tables."}' --account_id tilek.testnet
near call dev-1645348898006-52720569179472 addAnswer '{"answer":"Web 3.0 is a general idea for a decentralized Internet based on public blockchains"}' --account_id tilek.testnet

near call dev-1645348898006-52720569179472 deleteQuestion '{"question":1}' --account_id tilek.testnet
near call dev-1645348898006-52720569179472 deleteAnswer '{"answer":1}' --account_id tilek.testnet

near call dev-1645348898006-52720569179472 showMyQuestions --account_id tilek.testnet
near call dev-1645348898006-52720569179472 showMyAnswers --account_id tilek.testnet 

near call dev-1645348898006-52720569179472 getNumQuestions --account_id tilek.testnet
near call dev-1645348898006-52720569179472 getNumAnswers --account_id tilek.testnet 



--------------------------------------------------------------------------------------------

yarn test:unit