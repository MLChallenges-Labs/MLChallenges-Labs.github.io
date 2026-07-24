Many competitions are organized each year on platforms such as Kaggle, CodaLab Competitions or EvalAI. Some allow you to upload your model’s predictions, while others allow you to upload directly your model’s code to have it trained and tested on the platform. Which one is better? What should you do as a competition organizer? What are the pros and cons? Let’s have a closer look.



## Result submissions versus code submissions

Let’s end the suspense here. With the goal in mind to put in place a robust benchmark on a given problem, I advice for allowing only code submission, for the following reasons.

### Reproducibility

The first point is an improved reproducibility. With results submission, you can re-run the scoring involving the predictions and the ground-truth. This is quite limited, in comparison to code submission that you can re-run from scratch: the model training, making the predictions and then the scoring. Having the code at hand make a huge difference here. How can you know how the participants did obtain the predictions they submitted? You need them to tell you. Even if they do tell you, you need them to be specific enough in their description, and you need to trust them. Their predictions could even be made manually by a human, who knows? To perform rigorous experimental science, you must have the code of all algorithms that you compare, and being able to re-run all the experiments on the same environment.

### Complex Evaluation Procedures

A second point is the possibilities of running complex evaluation procedures. With code submission you can compute cross-validation, multiple trials, or even test the model in different conditions and on different hidden datasets. With results submission, the best you can do is using re-sampling (bootstrap) to compute errors bars.

### Control Cheating

It makes it easier to control cheating. If the participants submit their code, you can always review it to check that they are not doing anything forbidden by the rules of the challenge.

### Data Remain Hidden

Another point in favor of code submission is that your data are hidden for real, especially the test data. When allowing result submissions, you necessarily give access to X test, the test data given as input to the models to generate the predictions ŷ test! This is a huge bias as semi-supervised techniques can be used to fine tune the model, and increase the score specifically for the test data. More generally, code submission is less prone to data manipulation, and even allow you to use confidential data in the evaluation.

### Fairer

The last point I’ll make here is that code submission is fairer for the participants. It confers the exact same environment and the exact same computational resources to all candidates during the evaluation of submissions. It also allows to control the training and evaluation time. With result submission, participants are completely free. Of course, having a total liberty can be seen as an advantage: you can use all resources you have at hand to improve your score.

### Need to supply resources

The main disadvantage of code submission is that it requires from the organizer to supply resources. This can be very demanding as the number of participants and the complexity of the task increase. In this case, result submission help to decentralized the calculations into the computers of all candidates. It is a hard price to pay in order to have all the advantages mentioned above.



### Hard to put in place?

A common misconception about code submission is that it is tricky to put in place. It is usually not true. For instance, on CodaLab Competitions, it is actually extremely simple. This discussion is summed up in the table below.


| Criteria | Result Submission | Code Submission |
|--------|-------------------|-----------------|
| Information about the model |   | ✅ |
| Reproducible training |   | ✅ |
| Complete ecaluation   |   | ✅ |
| Control cheating |   | ✅ |
| Hidden data |   | ✅ |
| Equal resources |  | ✅ |
| Light computation | ✅ | ✅ |
| Easy to put in place | ✅ | ✅ |

*Main advantages and disadvantages of result submissions and code submissions.*

## Conclusion

To sum up, I think that competitions with code submission are the most serious ones, because it allows to perform systematic experiments, in a fair way for the participants. The main downside is that it requires more computing power on the side of the organizers. As Spider-Man said, “with great power comes great responsibility”.

*Original content by [Adrien Pavão](https://adrienpavao.com/).*
