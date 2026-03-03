Assessment
==========

Projects will be marked considering your team submission (code and report) and your project
presentation in unity.

You must submit code produced by you and your partner only; plagiarism of any kind (e.g. submission
of code not produced directly by your team) will be dealt with under university regulations. If any
third party library is used it needs to be clearly cited in your code. You must also flag any use of
third party library in your implementation before your presentation.

Your individual understanding of your implementation and principles of object orientation in
general, as well as the quality and clarity of the work conducted and depth of knowledge shown in
your presentation are considered for marking. A brief assessment guideline is provided below, also
giving details on the report. You can pass this coursework by submitting code that passes the tests,
and showing a good understanding of the code written and principles used. Note, that there are
limited and diminishing returns when implementing your AI solution, and we advise you to finish all
other parts first and make sure you are confident about the key principles of object-orientation and
Java before spending time on an AI solution.

Make sure you submit at least 1 hour early to avoid upload problems. Any submission after the
deadline will result in a loss of marks. Each team member has to upload an identical copy of the
submission zip file containing all of the work of the team. After the submission, each team will
present their work, where a time table for presentations will be published on the unit website. Both
team members must be present for the presentation. During the presentation we may run and discuss
your submitted program. You may run it on your own devices or the lab machines - you have to make
sure that your submitted program runs without problems. We will ask you questions about your work
and general principles of object-orientation and Java, and you will be able to showcase your
knowledge and the merits of your project. All team members should understand all code developed in
detail.

Vivas
==========

During your viva, **you must have your camera on and a working microphone**. Vivas will be around **20 minutes in duration** and will **take place on Teams**. You should have all your code ready to run. Remember, both team members may potentially receive different marks, so you’ll both need to answer questions in the viva.

To achieve a pass, you will only require a basic understanding of Java and have an implementation which passes the majority of tests. **However, if you cannot explain basic functionality of your code, you may not receive a passing grade - even with the all the tests passed and an advanced AI**.

Questions will be limited to content covered in the lectures (unless you know all of it!) and where possible will be themed around your implementation of the Scotland Yard model. For example, we might ask you to explain the following (going broadly from easier to harder):

* classes and objects
* attributes and methods
* instantiation and constructors
* access modifiers
* static methods
* immutables
* references and null
* generics
* overloading vs overriding
* getters, setters and encapsulation
* inheritance
* polymorphism and downcasting
* exceptions
* idea/code of observer
* abstract classes
* interfaces
* super
* dynamic dispatch
* idea/code of visitor
* MrX scoring function
* inner classes and anonymous classes
* initialisers ;;variadics
* basic design pattern knowledge about at least one pattern
* ...
* (and everything else we covered!)
* 
You may also be asked about later lecture content, including explaining more esoteric design patterns.

Remember, you *will* be asked to explain randomly selected sections of code implemented by your team.

Submission
==========
You should submit before the deadline (16/04/2026, 13:00), [HERE](https://www.ole.bris.ac.uk/ultra/courses/_264154_1/outline/assessment/test/_9730956_1?courseId=_264154_1&gradeitemView=details):

1. A brief **PDF** report (we expect this to be at least 1 page as a summary of what has been done,
   and 2 pages maximum reflecting on achievements. A strict maximum of 3 pages applies where the report should include some brief critical reflection on the merits and
   limitations of your work). **The file must be named report.pdf**
2. A compiling, building and running version of Scotland Yard including all source code to
   BlackBoard before the deadline in form of one single zip file called `sy.zip`. Your sub-projects
   `cw-model` and `cw-ai` must be in two different top level subfolders called `cw-model`
   and `cw-ai` within the zip file. Also include your `report.pdf` at the top level, next to `cw-model` and `cw-ai`.

Concretely, submit the following:

**Update: only submit 1 (one) file, `sy.zip` to BB, when you extract it, it should have the following structure:**

```
Submission 1:
 - sy.zip
   ├── report.pdf  # your PDF report
   ├── cw-model/   # root of the cw-model project, where running `mvnw clean test` will show all tests passing
   │    ├── mvnw
   │    ├── mvnw.cmd
   │    ├── pom.xml
   │    ├── src/
   │    └──  ...   # (any other file required for the project to compile can be in this directory)
   └── cw-ai/      # root of the cw-ai project, where running `mvnw clean compile exec:java` will run the project
        ├── mvnw
        ├── mvnw.cmd
        ├── pom.xml
        ├── src/
        └──  ...   # (any other file required for the project to compile can be in this directory)
```

**Failure to adhere to these requirements will result in loss of marks; we can't mark reports that
are not in PDF format or source files that are not compressed in zip format.**

Make sure you run the following of each of your sub-projects before submitting to remove compiled
binaries:

```shell
> mvnw clean
```

In any case, check that the version of your project resulting from unzipping your submission file
contains all source code and resources you created, that it compiles, passes all tests, and allows
you to run your game without the need for any other file outside your submission. The report does
not have to cover all things implemented in detail, but should be seen as an overview of the work
judged in conjunction with code and presentation - teams can use it during the presentation as an
aid. The report should be concise, clear and to the point.


Marking Guideline
=================

This mark scheme assesses two separate and equally weighted threads: **implementation depth** and **verbal demonstration of OO concepts**. To receive credit for any implementation work, students must **explain it clearly during the viva and run it successfully**; strong code without explanation earns little or no credit. Similarly, excellent verbally demonstrated OO knowledge can significantly raise the overall result. For example, a student passing only half the tests may score **40** for implementation but **80** for OO understanding, averaging **60**. However, a student unable to explain their code or core OO concepts will score **well below a pass**, regardless of code quality.

| **OOP Concepts Demonstrated** | **Assignment Implementation Achieved** | **Max Mark** |
|-------------------------------|----------------------------------------|--------------|
| - Basic OO: classes, objects, attributes, methods, encapsulation, with verbal understanding demonstrated<br>- Basic verbal understanding of OO concepts | - Project compiles<br>- Uses test suite<br>- Minimal documentation<br>- Basic report<br>- ~50% of tests passed | **40%** |
| - Good use **and verbal understanding** of OO concepts: overloading/overriding, immutables, generics<br>- Readable OO‑style reasoning (verbal) | - All model tests passed<br>- Good code documentation<br>- Concise report<br>- Evidence of individual contributions | **55%** |
| - Good verbal understanding of observer pattern<br>- Good verbal understanding of polymorphism, abstraction, DRY principles<br>- Solid understanding of all basic OO concepts | - Well‑structured OO‑style code<br>- DRY code | **60%** |
| - Good verbal understanding of dynamic dispatch<br>- Good verbal understanding of visitor pattern<br>- Broad verbal understanding of OO concepts | - Simple MrX scoring function implemented<br>- Good report<br>- Productive individual contributions | **65%** |
| - Very good verbal understanding of most OO concepts<br>- Some verbal understanding of design patterns | - Effective, well‑tested scoring function<br>- Very well‑documented code<br>- Follows very good coding practices<br>- Very well‑written report | **70%** |
| - Excellent verbal understanding of OO concepts<br>- Good verbal understanding of a variety of design patterns<br>- Strong ability to articulate and justify OO design decisions | - Distance‑based Look‑Ahead‑One AI implemented<br>- Excellently written and critically reflective report<br>- Strong individual contributions | **75%** |
| - Critical, appropriate verbal understanding of design patterns<br>- Excellent OO reasoning and architecture explained verbally | - MrX AI uses MiniMax or similar game‑tree search<br>- Excellent work, presentation and report<br>- Evidence of excellence in individual contributions | **80%** |
| - Exceptional verbal command of OO theory and advanced design patterns<br>- Deep, articulate insights into architecture and design | - AI beyond MiniMax (more efficient/dynamic algorithm)<br>- Exceptional work, presentation and report<br>- Outstanding individual contributions | **87%** |
| - Mastery and critical verbal understanding of OO and design patterns beyond course content<br>- Research-level conceptual insight | - Outstanding extensions and advanced methods<br>- Publishable‑quality product<br>- Outstanding report and presentation<br>- Exceptional individual contributions | **100%** |
