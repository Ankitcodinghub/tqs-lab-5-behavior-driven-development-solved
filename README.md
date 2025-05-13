# tqs-lab-5-behavior-driven-development-solved
**TO GET THIS SOLUTION VISIT:** [TQS Lab 5-Behavior-driven development Solved](https://www.ankitcodinghub.com/product/tqs-lab-5-behavior-driven-development-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93893&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;TQS Lab 5-Behavior-driven development Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 14">
<div class="layoutArea">
<div class="column">
Lab 5 Behavior-driven development (Cucumber in Java)

Context and key points

Prepare

Keep in mind that the integration of JUnit 5 and Cucumber is still somewhat recent and most of the samples available on the internet are still based on JUnit 4. While this is correct and possible, we will try to stick with JUnit v5 and the test runtime engine.

You may configure InteliJ to offer extended support to run Cucumber.

Key Points

<ul>
<li>⎯ &nbsp;The Cucumber framework enables the concept of “executable specifications”: with Cucumber we use examples to specify what we want the software to do. Scenarios are written before production code.</li>
<li>⎯ &nbsp;Cucumber executes features (test scenarios) written with the Gherkin language (readable by non-programmers too).</li>
<li>⎯ &nbsp;The steps included in the feature description (scenario) must be mapped into Java test code by annotating test methods with matching “expressions”. Expressions can be (traditional) regular expressions or the (new) Cucumber expressions.
Explore

<ul>
<li>Cucumber school: guided exercises, video lessons,…</li>
<li>BDD with Cucumber – video presentation.</li>
</ul>
</li>
</ul>
5.1 Getting started

The Cucumber for Java platform has frequent updates that, sometimes, change the “best practices” to prepare the test scripts.

<ol>
<li>a) &nbsp;Get the “Java Skelton” project proposed by Cucumber.

Adjust the compiler version in the POM (1.8 → 11). You may also change the Artifact group and Id.</li>
<li>b) &nbsp;Note some elements I the POM:</li>
</ol>
&lt;dependencyManagement&gt; with *-bom There are “bills of materials”. Their use in the

entries. Dependency management section is useful to enforce the

</div>
</div>
<div class="layoutArea">
<div class="column">
14 | TQS LABS

</div>
</div>
</div>
<div class="page" title="Page 15">
<div class="layoutArea">
<div class="column">
45426 Teste e Qualidade de Software

</div>
</div>
<div class="layoutArea">
<div class="column">
maven-compiler-plugin

</div>
<div class="column">
coherent use of the versions of related artifacts. Note that in the &lt;dependencies&gt; section, the related artifacts omit the version specification.

Sometimes, to use more recent constructions, you may need to control the maven compiler version.

</div>
</div>
<div class="layoutArea">
<div class="column">
c) Note the project structure, identify the location of the features and the tests.

A feature will typical matcha a “test runner” class thar will activate the test steps (in the same package).

The “test runner” class (that runs the test) should be annotated with:

@Suite

@IncludeEngines(“cucumber”) @SelectClasspathResource(“my/package/structure”)

<ol start="4">
<li>d) &nbsp;Run the tests.

The tests will not pass because they still are incomplete.

Note the “clues” in the output, giving suggestions to

implement the missing steps (i.e., test methods). Use these suggestions to create the missing steps. Note that, for this purpose, the “Belly” class implementation can just log information.
</li>
<li>e) &nbsp;Extend your project to include also the Calculator example discussed in “Cucumber in a Nutshell” section in B. Garcia’s book4.
Note1: the example just some sample code that uses old-style integration with JUnit. You should adopt the strategy for the previous [skeleton] example. No new imports or dependencies required!

Note2: in this example, the steps matching uses regular expressions. The best practice, however, is to use “cucumber expressions”. Be sure to “upgrade”. E.g.:

Regular expressions style Cucumber expressions style [better] @When(“^I add (\\d+) and (\\d+)$”) @When(“I add {int} and {int}”)
</li>
</ol>
5.2 Books

To get into the “spirit” of BDD, partner with a colleague, and jointly write a couple of features to verify a book search user story. Consider a few search options (by author, by category, etc).

Take the approach discussed in this example, and write your own tests. Feel free to add different scenarios/features.

Notes:

<ul>
<li>– &nbsp;The article is based on old-style Cucumber constructions. Ignore the dependencies and annotations suggested in the text: use the “Skeleton” exercise as a reference for Cucumber dependencies and test annotations.</li>
<li>– &nbsp;Write the features before the test steps. Steps can be partially generated from features.</li>
<li>– &nbsp;Prefer the “cucumber expressions” (instead of regular expressions) to write the steps definitions.</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
4 solution code available, if needed.

</div>
</div>
<div class="layoutArea">
<div class="column">
TQS LABS | 15

</div>
</div>
</div>
<div class="page" title="Page 16">
<div class="layoutArea">
<div class="column">
<ul>
<li>– &nbsp;To handle dates, consider using a ParameterType configuration. This defines a new custom parameter type to use in the matching expressions . [ → partial snippet]. The dates in the feature description need also to match the date mask used (aaaa-mm-dd).</li>
<li>– &nbsp;To handle data tables in the feature description (as in the Salary manager example), consider using a DataTable mapping and access you data as a list of maps (use headings in the data).</li>
</ul>
5.3 Web automation

Cucumber can be used with Selenium WebDriver to write expressive automation tests.

Consider the example available in B. Garcia’s repository concerning the integration of Cucumber and Selenium [junit5-cucumber-selenium] and implement it.

Adapt from this example to create a test scenario related to the “BlazeDemo” application (recall Lab 4, exercise 2).

</div>
</div>
</div>
