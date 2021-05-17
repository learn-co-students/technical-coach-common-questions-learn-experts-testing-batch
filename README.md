# Common Questions

![questions](http://i.giphy.com/xTk9ZMytZS75B48rD2.gif "questions")

As a Technical Coach, you’ll get all sorts of question from all sorts of different students. It can be overwhelming to have to constantly switch contexts (in terms of the student, the topic, and the question). Broadly speaking, the questions will fall into one of more of the five categories listed below:

* **Learn/IDE/Workflow issues**
* **Lab tests don't run**
* **Tests run but student gets error messages they don’t know how to fix**
* **Conceptual questions**
* **Unsupported questions**

For each category of question, we’ve given examples as well as specific strategies you can use to resolve them.

## 1) Learn/IDE/Workflow Issues

### Issue
Problems with the platform and workflow (lights/IDE/empty cloned directory/etc)

### Common Examples
* Lights do not turn green
* `learn open` and `learn submit` do not work
* The lesson directory is empty
* When submitting lessons, the student is asked to enter their username and password

### Strategies for Resolution
Solve the problem for the student - often the Learn.co help articles or the `#tc_support` channel will have fixes for platform-related issues. If you're not able to resolve the issue, file a ticket if necessary, and get the student to move on if possible.

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
* Infinite loop
* Lab requires some code to be written before tests will run

### Strategies for Resolution
*  **If it's an environment issue**:, we can solve it for the student. Take a few minutes to investigate and see if you understand what the problem is. If you do, then tell the student first, in one or two sentences, what the error is. After that tell the student that you will walk them through the steps to fix if it’s short. If it's more complicated, you can do it for them over screen share. Again, check the help articles or `#tc_support` if you're not sure how to proceed, or google the error. If it's an error related to Virtual Box, [check out this article about common VB Errors and related resources](https://github.com/flatiron-labs/technical-coach-resources/blob/master/virtual-box-setup-errors-and-resources.md).

    - For example, if it’s an issue with their gems and they need to run `bundle install`, tell them explicitly what the problem is and then say, "Okay, here are the steps to fix it and we’ll see what happens".
    - Walk them through the commands. Depending on how long the process took, end this with a debrief of what you just did.
    - Send any helpful links or resources that the student can use as a reference.

* **If it's a syntax error**: and you know that it’s something that the student did wrong with their code, then employ teaching strategies to solve it (e.g. the Socratic Method). Read through the error and ask the student if they know what this error means. If the student doesn’t know within three questions of you asking, then point it out specifically. Then tell them to look through their code and see if they are missing anything and have them re-run it. After 10 minutes of this, if they’re still stuck, have them ask you again. At this point, you can provide them with the answer. A lot of times the error will tell you what line has a syntax issue. Make sure you point this out to the student and show them how you are solving it, so they can replicate your technique! *(Example: running a chunk of problem code in IRB or Chrome console)*.

* **If it's an infinite loop**: In this case, the tests will often "hang" on one test and/or the tests will behave as if the student has passed the lab, even if it is clearly not complete. Employ teaching strategies as you would with a syntax error - help students identify in which method the tests seem to "hang", and use questioning techniques to help identify why their looping condition is always true, and how you might resolve that. Having the student walk through their loop line by line with you can help them realize the problem, or use a debugging tool like pry to help visualize how their data is or isn't updating.

*  **Some labs require the student to start coding before they can run the tests**: For example, some of the Sinatra labs require some migrations to be written first - otherwise, the student will get strange error messages when running the tests. You may need to probe to determine if this is the case or if it's an environment issue. If the lab does require the student to write some code, employ teaching strategies to get the student to fix it. You may need to redirect students to the readme as well, as often students will miss a step in the instructions.

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

* **Walk students through their error message**: Have the student walk you through the specific steps slowly and reinforce with a simple “yes” or “good” each time they explain something correctly. If there is an error in their explanation, you should point out that what they’re explaining or doing isn’t correct - but don’t give them the answer. Ask them questions and see if they can self-correct. If they have trouble, then walk them specifically through the different parts of the error message and decode it for them. At the end of this, have them repeat the meaning of the error message to you.

* **Walk students through their code**:  Once they understand the error message, go to the relevant code and ask them first if they can see what's wrong. Follow the same steps above to see if they can self-correct first. If they don’t see what’s wrong, ask them what they should do to fix the error. They may not know the specific step, but see if you can get to a general understanding of the issue.

* **Google**: At this point, if they can’t solve it and it’s a simple solution or requires a quick lookup in the docs, have them google it. *Do not, however, say “Google it.”* A student might think you’re trying to avoid helping them by saying that. Instead, help them with terms and specific vocabulary. You want to teach them how to Google. A helpful comment, for example, could be “Let's try googling 'ActiveRecord validations Rails'". Ask the student if that’s helpful and if they know what their next steps are. Ensure they have a plan for dealing with the problem, and tell them to follow up with you within 15 minutes. See if you can provide them with enough info to have them Google the problem.  Or you can follow up with them in 15 minutes to check in and say something like, “Did you figure out the validation issue you were having?". This lets them know that you haven’t forgotten them. If you're on a screen share, you can guide them through the googling process but don't do it for them.

* **Give students information they need**: At some point if students are still struggling - usually after three or four questions that they don’t know how to answer- you will want to supply them with the answer. Use your judgement though. If you feel like this is a productive question-and-answer session for the student and they're getting closer to solving the problem, then continue. Otherwise, you may want to supply the answer to the question and tell the student what to do to get the test to pass. Be sure to explain why that solution works. The important thing is to feel that you’ve done enough to augment their understanding.

* **Have students debrief you**: At the end, have the student debrief you on what they did and why it worked. Tell them they can take their time and that their response does not have to be just a sentence or two. Tell them you want them to really think through the error message and what they did to get their tests to pass. This is important because you want them to reflect on their learning. If it ended up being something you ultimately provided the answer to, this will still ensure they think about what happened.

If a student has multiple test failures, then after you’ve helped them solve one of them, tell the student to try and solve the next error(s) on their own. If they get stuck, then they can come back and ask additional questions, but they should try to debug and Google on their own for at least 15-30 minutes.

By using the Socratic method, you may realize early on that the problem isn’t about questions with error messages, but rather about larger conceptual issues they are confused about.

In this case, review the strategies for fixing conceptual questions listed below.

## 4) Conceptual Questions

### Issue

Students are struggling to understand the broader or underlying concepts that were covered, not specific tests.

### Common Examples

* Students do not understand the instructions of a lab
* Students do not understand one specific instruction or how to get a test to pass on a lab
* Students ask about a specific concept
* Students may initially have questions about failing tests, but after you’ve debugged and worked with them, you realize there are larger concepts that they don’t understand fully. (e.g. You're working on rails form helpers and then realize that they have no idea what `params` is)

### Strategies for Resolution

* **Link them to a video or resource**: Some common or beginner conceptual issues can be resolved by linking the student to a pre-recorded video we have in our video archive, [which you can access here](http://instruction.learn.co). You can also feel free to link them to a relevant YouTube video, documentation, or other resource (e.g. a relevant blog post or W3Schools article).

* **Teaching mode**: You can try and solve the student’s issue through a comprehensive walkthrough of the concept. Pull out from the context of the specific lesson the student is working with and give other code examples of the concept. For example, if is student is struggling to apply an enumerable method to their code, you could provide a simple example of operating on a dummy array with the same method.   

You can ask the student to explain the underlying concept or more specifically, ask the student why the result is what it is and then have them elicit the rules from there. Once you know where they’re having trouble,  break down the concept into smaller components and explain how these components build on top of each other. Start with the most basic component and use short concept questions to check to see what the student does know. Concept questions are simple and straightforward and usually require a yes/no or short answer.

At some point you’ll see where exactly the student is lost. From there, take the reins and continue demoing the rest of the concept as slowly and as clearly as possible. Every few minutes, check to make sure that the student understands what you’re presenting or if they need clarification. At the end of the demo, have the student summarize the concept.

* **Document the issue**: After explaining the concept, if the student still doesn't understand, document the issue in their admin profile. Click on their icon at the top of their question in Pair with a Coach to get to the student’s `/admin` page. Make a note that the student is having an issue with the specific concept and explain where they're lost and what you steps you took to try to explain the issue, as well as any other relevant info.

* **Escalate the issue**: If you see other TCs have already pointed out that this student doesn’t understand the concept, or is struggling in general with concepts covered in their current section, [escalate the student](https://docs.google.com/forms/u/1/d/e/1FAIpQLSdIP65BStJfWBgG0dZO5dhQb3Yqs3TwN29xjk5GUOyyReI5QQ/viewform). **Note: If it's a paying student, it is especially important to leave a note in their admin profile and escalate the student.** Escalating the student alerts the Faculty Manager and other full time staff that the student is in need of additional support, while leaving a note on the student's profile 1) makes other TCs aware of issues the student is having, and 2) helps to document persistent issues.

As with any student escalation, you want to be as clear and objective as possible. Give examples to illustrate what the student is struggling with, and describe how you tried to teach the student the concept, and what the outcome was. Quote the student if it is appropriate, particularly if the student is expressing frustration or feelings about giving up.

**Video Example** [Student is having issues conceptually and needs guidance to get on the right track](https://youtu.be/q2WoFBdyXxI)

## 5) Unsupported

### Issue

We don't support these types of questions. These questions are usually regarding assessments, but sometimes other issues, too.

### Common Examples

* Questions about admissions
* Questions about billing
* Help with assessments / portfolio projects
* Help with non-curriculum code ( e.g. a side project )

### Strategies for Resolution

* **Admissions or billing questions**: Questions regarding admissions or billing can be referred to the Admissions department. This can be done by clicking on the `Assign to Enrollments` button in the bottom of the chat window, between `Resolve` and `Log Bug Report`. Let the student know that this will resolve the question and that they should hear back from someone within 24 hours. You can also advise students to reach out to admissions directly at `admissions@flatironschool.com`. Other questions that are not related to admissions but are not related to labs or lessons (Slack access, access to specific tracks, etc.) can be directed to our Student Services department at `studentservices@flatiron.com`.

* **Assessment questions**: We use assessments to see how a student has done in a specific topic, and instructors will pair with students and assess their skills. Because of this, students should not be asking Technical Coaches for help with their assessment project. There are a number of solutions for handling assessment questions, so be sure to make students aware of their options:
  * **Dedicated Project Support**: _Always_ refer students to the appropriate contact person(s) for project support, so that they do not feel like we do not want to help them, or that there is no appropriate avenue for them to get help. There are two general places to refer students to get project help, depending on whether they are in a structured or a self-paced program. It is very important to refer students to the correct place, so if you're unsure, ask your fellow TCs! If a student becomes especially frustrated about not being able to get project support or is rude, please escalate them [here](https://docs.google.com/forms/u/1/d/e/1FAIpQLSdIP65BStJfWBgG0dZO5dhQb3Yqs3TwN29xjk5GUOyyReI5QQ/viewform) and quote them directly.
    * **Students in a structured (part time or full time) program**: refer the student to their cohort lead - they should already know the name of their cohort lead and how to contact them.
    * **Students in the self-paced program**: Refer students to their Section Lead and Section Coach - they can find the Section Leads and Section Coaches [here](https://help.learn.co/en/articles/492988-who-are-the-section-leads). Students can reach out to any and all staff members at that link who teach their current section (e.g. javascript). Students can reach out to their Lead/Coach via the listed emails, or can also reach out via slack by searching the staff member's name.
  * **Instructional Videos**: There are quite a few videos students can search through at [http://instruction.learn.co](http://instruction.learn.co). This is a great resource for students as they work on their projects - in addition to videos covering general concepts, there are also videos covering projects specifically.
  * **Study Groups**: Students can check out some of the study groups we run every week, some of which are dedicated specifically to project questions. This is a great time to learn about a particular coding concept or to ask questions to a live Section Lead or Section Coach. Generally students will receive alerts or emails about study groups for their current section, but they can also see the study group schedule [here](https://learn.co/study-groups).
  * **Slack Channels**: It is fairly common for students to ask for and receive help in many of the Slack channels - there are cohort-specific channels for students in structured programs, section-specific channels (e.g. `rails-section`) channels for self-paced students, and a number of channels that should be accessible to all paying students (e.g. `general` or `nerdy-learn-neighbors`).

* **All other questions**: Tell them we don't support the question type. We never want to annoy or add to a student's frustration so be kind and friendly when speaking with them. For questions that are unrelated to admissions, assessments, labs, or lessons - kindly tell them we don't support the question they're asking. The safest bet might be to refer them to Student Services at `studentservices@flatiron.com`, unless they are working on an outside project unrelated to any portfolio project, which we cannot support at all.

## Resources

* [Common VB Errors and related resources](https://github.com/flatiron-labs/technical-coach-resources/blob/master/virtual-box-setup-errors-and-resources.md)
* [Instructional Videos](http://instruction.learn.co)
* [Portfolio Project Support Help Center Article](http://help.learn.co/instructional-support/receiving-course-support/who-can-i-contact-for-help-on-my-portfolio-project)
* [Section Leads and Section Coaches](https://help.learn.co/en/articles/492988-who-are-the-section-leads)
* [Study Group Schedule](https://learn.co/study-groups)
* [Student Escalation Form](https://docs.google.com/forms/u/1/d/e/1FAIpQLSdIP65BStJfWBgG0dZO5dhQb3Yqs3TwN29xjk5GUOyyReI5QQ/viewform)
