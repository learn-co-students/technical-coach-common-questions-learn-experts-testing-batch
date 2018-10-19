# Common Questions

![questions](http://i.giphy.com/xTk9ZMytZS75B48rD2.gif "questions")

As a Technical Coach, you’ll get all sorts of question from all sorts of different students. It can be overwhelming to have to constantly switch contexts (in terms of the student, the topic, and the question). Broadly speaking, the questions will fall into one of more of the five categories listed below:

* **Learn/IDE/Workflow Issues**
* **Lab tests don't run**
* **Tests run but student gets error messages they don’t know how to fix**
* **Conceptual questions**
* **Unsupported questions**

For each category of question, we’ve given examples as well as specific strategies you can use to resolve them. 

## 1) Learn/IDE/Workflow Issues

### Issue
Problems with the platform and workflow (lights/IDE/empty cloned directory/billing/etc) 

### Common Examples
* Lights do not turn green
* `learn open` and `learn submit` do not work
* The lesson directory is empty
* When submitting lessons, the student is asked to enter their username and password 

### Strategies for Resolution
Solve the problem for the student or if they can keep moving on in the curriculum, tell them to just keep going. Report a bug if needed, but get the student to move on if possible.

These questions are not related to the specific content of the lesson but are usually issues students are having that are preventing them from moving forward. With these questions, the goal is to resolve them as quickly as possible so they can continue working on the lessons.

Don’t worry about using the Socratic method or making this a learning experience. In many cases, you’ll be telling students exactly what to do. Sometimes at the end you can send them links or resources that might be helpful in giving them a better understanding of the problem or for them to use as a reference in the future.

In some cases, you might not be able to solve the problem for them but if they’re still able to progress in the curriculum content, then you can tell them to move on. If not, you may need to escalate the issue to the development team (more on this later).

**Video Example** [technical coach helping a student understand technical issues](https://youtu.be/0Rege7kJoM8)

## 2) Lab tests don't run

![tests dont run](http://i.giphy.com/qvSGXu0VdKMBa.gif "Tests dont run")

### Issue
Environment or syntax errors or program breaks when running tests.

### Common Causes
* Environment / dependency issue
* Syntax error
* Lab requires some code to be written before tests will run

### Strategies for Resolution
*  **If it's an environment issue**, we can solve it for the student. Take a few minutes to investigate and see if you understand what the problem is. If you do, then tell the student first, in one or two sentences, what the error is. After, that tell the student that you will walk them through the steps to fix if it’s short. If it's more complicated, you can do it for them over screen share. If it's an error related to Virtual Box, [check out this articles about common VB Errors and related resources](https://github.com/flatiron-labs/technical-coach-resources/blob/master/virtual-box-setup-errors-and-resources.md).

    - For example, if it’s an issue with their gems and they need to run `bundle install`, tell them explicitly what the problem is and then say, "Okay, here are the steps to fix it and we’ll see what happens". 
    - Walk them through the commands. Depending on how long the process took, end this with a debrief of what you just did.
    - Send any helpful links or resources that the student can use as a reference.

* **If it's a syntax error** and you know that it’s something that the student did wrong with their code, then employ teaching strategies to solve it (eg the Socratic Method). Read through the error and ask the student if they know what this error means. If the student doesn’t know within three questions of you asking, then point it out specifically. Then tell them to look through their code and see if they are missing anything and have them re-run it. After 10 minutes of this, if they’re still stuck, have them ask you again. At this point, you can provide them with the answer. A lot of times the error will tell you what line has a syntax issue. Make sure you point this out to the student and show them how you are solving it, so they can replicate your technique! *(Example: running a chunk of problem code in IRB or Chrome console)*.

*  **Some labs require the student to start coding before they can run the tests**. For example, some of the Sinatra labs require some migrations to be written first - otherwise, the student will get strange error messages when running the tests. You may need to probe to determine if this is the case or it's an environment issue. If the lab does require the student to write some code, employ teaching strategies to get the student to fix it.

## 3) Tests run but student gets error messages they don’t know how to fix

![tests fail](http://i.giphy.com/xT8qB2HYA1vVSxooSY.gif "Tests fail")

### Issue

Pretty self-explanatory from above title. This is good though - everything is working! But students are confused about the code. This is where actual learning can happen. As a Technical Coach, you will use a variety of strategies to get students to the point where they know what they need to do to get their tests to pass.

### Common Examples

* Student doesn’t know why their tests aren’t passing
* Student doesn’t understand what the error message means
* Student doesn’t know what the test requires
* Student isn’t sure what the next step in the debugging process is

### Strategies for Resolution

* **Walk students through their error message**: Have the student walk you through the specific steps slowly and reinforce with a simple “yes” or “good” each time they explain something correctly. At the point of the error, you should point out that what they’re explaining or doing isn’t correct but don’t give them the answer. Ask them questions and see if they can self-correct. If they have trouble, then walk them specifically through the different parts of the error message and decode it for them. At the end of this, have them repeat the meaning of the error message to you.

* **Walk students through their code**:  Once they understand the error message, go to the relevant code and ask them first if they can see what's wrong. Follow the same steps above to see if they can self-correct first. If they don’t see what’s wrong, ask them what they should do to fix the error. They may not know the specific step, but see if you can get to a general understanding of the issue.

* **Google**: At this point, if they can’t solve it and it’s a simple solution or requires a quick lookup in the docs, have them google it. *Do not, however, say “Google it.”* A student might think you’re trying to avoid helping them by saying that. Instead, help them with terms and specific vocabulary. You want to teach them how to Google. A helpful comment, for example, could be “Let's try googling 'ActiveRecord validations Rails'". Ask the student if that’s helpful and if they know what their next steps are. Ensure they have a plan for dealing with the problem, and tell them to follow up with you within 15 minutes. See if you can provide them with enough info to have them Google the problem.  Or you can follow up with them in 15 minutes to check in and say something like, “Did you figure out the validation issue you were having?". This lets them know that you haven’t forgotten them. If you're on a screenshare, you can guide them through the googling process but don't do it for them.

* **Give students information they need**: At some point if students are still struggling - usually after three or four questions that they don’t know how to answer- you will want to supply them with the answer. Use your judgement though. If you feel like this is a productive question-and-answer session for the student and they're getting closer to solving the problem, then continue. Otherwise, you may want to supply the answer to the question and tell the student what to do to get the test to pass. Be sure to explain why that solution works. The important thing is to feel that you’ve done enough to augment their understanding.

* **Have students debrief you**: At the end, have the student debrief you on what they did and why it worked. Tell them they can take their time and that their response does not have to be just a sentence or two. Tell them you want them to really think through the error message and what they did to get their tests to pass. This is important because you want them to reflect on their learning. If it ended up being something you ultimately provided the answer to, this will still ensure they think about what happened.

If a student has multiple test failures, then after you’ve helped them solve one of them, tell the student to try and solve the next error(s) on their own. If they get stuck, then they can come back and ask additional questions, but they should try to debug and Google on their own for at least 15-30 minutes.

By using the Socratic method, you may realize early on that the problem isn’t about questions with error messages, but rather about larger conceptual issues they are confused about.

In this case, review the strategies for fixing conceptual questions listed below.

## 4) Conceptual Questions

### Issue

Students are struggling the broader or underlying concepts that were covered, not specific tests. 

### Common Examples

* Students do not understand the instructions of a lab
* Students do not understand one specific instruction or how to get a test to pass on a lab
* Students ask about a specific concept
* Students may initially have questions about failing tests, but after you’ve debugged and worked with them, you realize there are larger concepts that they don’t understand fully. (eg You're working on rails form helpers and then realize that they have no idea what `params` is)

### Strategies for Resolution

* **Link them to a video**: Some common or beginner conceptual issues can be resolved by linking the student to a pre-recorded video we have in our video archive, [which you can access here](http://instruction.learn.co).

* **Teaching mode**: You can try and solve the student’s issue through a comprehensive walkthrough of the concept. Pull out from the context of the specific lesson the student is working with and give other code examples of the concept. Ask the student to explain the underlying concept or more specifically, ask the student why the result is what it is and then have them elicit the rules from there. Once you know where they’re having trouble,  break down the concept into smaller components and explain how these components build on top of each other. Start with the most basic component and use short concept questions to check to see what the student does know. Concept questions are simple and straightforward and usually require a yes/no or short answer. At some point you’ll see where exactly the student is lost. From there, take the reins and continue demoing the rest of the concept, slowly and as clearly as possible. Every few minutes, check to make sure that the student understands what you’re presenting or if they need clarification. At the end of the demo, have the student summarize the concept. 

* **Document the issue**: After explaining the concept, if the student still doesn't understand, document the issue in their admin profile. Click on their icon in at the top of their question in AAQ to get to the student’s `/admin` page. Make a note that the student is having an issue with the specific concept and explain where they're lost and what you steps you took to try to explain the issue, as well as any other relevant info.

* **Escalate the issue**: If you see other TCs have already pointed out that this student doesn’t understand the concept, [fill out the Additional Support form noted in this article](https://github.com/flatiron-labs/technical-coach-resources/blob/master/feedback.md). **Note: If it's a paying student, it is especially important to leave a note in their admin profile and email or Slack the Faculty Manager, the Section Lead, or their Cohort Lead so we can get this student additional help!**

**Video Example** [Student is having issues conceptually and needs guidance to get on the right track](https://youtu.be/q2WoFBdyXxI)

## 5) Unsupported

### Issue

We don't support these types of questions. These questions are usually regarding assessments, but sometimes other issues too.

### Common Examples

* Questions about admissions
* Questions about billing
* Help with assessments / portfolio projects
* Help with non-curriculum code ( eg a side project )

### Strategies for Resolution

* **Admissions or billing questions**: Questions regarding admissions or billing can be referred to the admission department. This can be done by clicking on the `Assign to enrollments` button in the bottom of the chat window, between `Resolve` and `Log Bug Report`. Let the student know that this will resolve the question and that they should hear back from someone within 24 hours. 

* **Assessment questions**: We use assessments to see how a student has done in a specific topic and instructors will pair with students and assess their skills. Because of this, students should not be asking Technical Coaches for help with their assessment project. There are a number of solutions for handling assessment questions, listed below in order of precedence.
  * **Instructional Videos**: There are quite a few videos you can search through at [http://instruction.learn.co](http://instruction.learn.co). This is a great resource that the student should check first.
  * **Study Groups**: If none of the videos were helpful and they're still stuck on a particular concept, suggest they check out some of the Study Groups we run every week. This is a great time to learn about a particular concept as well be able to ask questions to a live Technical Coach.

  **10/19/18: The following solutions are being phased out. Please consult with your TCL before doing either of these.**
  * **1:1 Portfolio Support**: If neither videos nor Study Groups were able to resolve the student's problem, have them schedule a 30 minute 1:1 session with a portfolio coach](https://theflatironschool.typeform.com/to/UUhrc7). For more info and the link to book a session, you can check out this article on the help center: http://help.learn.co/instructional-support/receiving-course-support/who-can-i-contact-for-help-on-my-portfolio-project
  * **DM the Section Lead**: If the student is still struggling, even after a 1:1 portfolio support session, they can contact the [section lead](https://github.com/flatiron-labs/technical-coach-resources/blob/master/section-leads.md) for that particular section.

* **All other questions**: Tell them we don't support the question type. We never want to annoy or add to a student's frustration so be kind and friendly when speaking with them. For questions that are unrelated to admissions or assessments, kindly tell them we don't support the question they're asking. If the question is related to the curriculum, feel free to answer it if time is available. Otherwise you may want to give them a link to a resource or point them in the direction they should proceed (eg try googling it, checking stack overflow, asking in the Slack channel, etc).


## Resources

* [Common VB Errors and related resources](https://github.com/flatiron-labs/technical-coach-resources/blob/master/virtual-box-setup-errors-and-resources.md)
* [Instructional Videos](http://instruction.learn.co)
* [Portfolio Project Support Help Center Article](http://help.learn.co/instructional-support/receiving-course-support/who-can-i-contact-for-help-on-my-portfolio-project)
* [Portfolio Project Support Form](https://theflatironschool.typeform.com/to/UUhrc7)
* [Section leads](https://github.com/flatiron-labs/technical-coach-resources/blob/master/section-leads.md) 
