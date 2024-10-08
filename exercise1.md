# Answers for Exercise 11.1
> [!TIP] Here, I left a reference for the question I am answering.

The answers (my text) is right below, just like this text. Sorry for the formatting, but I am just trying to make my text a bit neat.

----
**Generals:-**
Language I picked, `Ruby`
My Knowledge on The Language: `~2%`
Words Count: `298`

----

> [!TIP] **Some common steps in a CI setup include linting, testing, and building. What are the specific tools for taking care of these steps in the ecosystem of the language you picked?**

**Building:** As an interpreted language, Ruby doesn't need a building step. We can run it using the `make` command in the terminal or 
```
ruby filename.rb
```

**Linting:** The most famous options are [RuboCop](https://github.com/rubocop/rubocop), which is known for its full developer-based configurations allowing more control and creating extra complexity, and [StandardRB](https://github.com/testdouble/standard) known for its pre-defined common standards. 

**Testing:** Options are [RSpec](https://rspec.info/) known as a great and easy-to-understand behavior-driven development (BDD) framework and [Minitest](https://docs.seattlerb.org/minitest/) known for its versatile testing style (allowing for BDD testing style or the traditional unit-testing style).


----

> [!TIP] **What alternatives are there to set up the CI besides Jenkins and GitHub Actions?**

To mention a few, these were the first I found:
- CircleCI
- Gitlab CI
- Bitbucket Pipelines
- AWS CodePipeline
- Azure DevOps
- GoCD
- TeamCity
- Bamboo
- Harness
- Spinnaker

----

> [!TIP] **Would this setup be better in a self-hosted or a cloud-based environment?**

For a team of ~6 developers nearing release, a cloud-based CI is more ideal.

> [!TIP] **Why?**

Surly, setting up a local CI would require extra management and setup time, additional expertise for server management, huge investments, and complexity once scaling up/down the resources.

Unless the team is big or there are sensitive data that shouldn't go online, a cloud-based option would definitely be a better option.

> [!TIP] **What information would you need to make that decision?**

I need to know the team size, deployment frequency, budget, security requirements, resource requirements (like a GPU), and the project's end vision. 

If the project would end-up being open source, then it should definitely have a cloud-based CI! And if the budget for the project is tight, the local option would be costing quite much (from setup and maintenance time to hardware needs).

Same idea on the team and how often would they deploy since that would affect the cloud-based costs. If it would be too much deployments for a 50+ developers team (in different time zones) and it would be better to go for a local option in that case.