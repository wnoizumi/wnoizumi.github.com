<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <meta name="description" content="Graph-based visualization for code smell agglomerations: A controlled experiment">
    <meta name="author" content="O. I. A. Benedicte Agbachi">

    <title>VEM 2017 - SUBMISSION: Graph-based visualization for code smell agglomerations: A controlled experiment</title>

    <!-- Bootstrap core CSS -->
    <link href="bower_components/bootstrap/dist/css/bootstrap.min.css" rel="stylesheet">

    <!-- Custom styles for this template -->
    <link href="grid.css" rel="stylesheet">

    <link rel="stylesheet" type="text/css" href="design.css">

    <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
    <!--[if lt IE 9]>
      <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
      <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
    <![endif]-->
    <link rel="stylesheet" href="bower_components/highlightjs/styles/xcode.css">
    <script src="bower_components/highlightjs/highlight.pack.min.js"></script>
    <script src="bower_components/jquery/dist/jquery.min.js"></script>
    <script src="bower_components/bootstrap/dist/js/bootstrap.min.js"></script>
    <script>
        hljs.initHighlightingOnLoad();
    </script>

    <style type="text/css">
        pre {
            border: none;
            background: #ffffff;
            padding: 0px;
        }
        
        .col-md-6 {
            background: #ffffff;
            border: none;
            padding-bottom: 0px;
        }
        
        body {
            padding-top: 70px;
            position: relative;
        }
    </style>

    <script type="text/javascript">
        $(document).ready(function() {
            $('body').scrollspy({
                target: '#mainNavBar'
            })
        });
    </script>
</head>

<body>
    <nav id="mainNavBar" class="navbar navbar-default navbar-fixed-top">
        <div class="container-fluid">

            <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-6">
                <ul class="nav navbar-nav">
                    <li><a href="#abstract">Abstract</a></li>
                    <li><a href="#dp">Design Problems</a></li>
                    <li><a href="agglomerations">Categories of Agglomerations</a></li>
                    <li><a href="#selection">Participant Selection</a></li>
                    <li></li>
                <!--    <li><a href="#procedures">Procedures on Communicability Evaluation</a></li> -->
                    <li><a href="#download">Download</a></li>
                    <li><a href="#references">References</a></li>
                </ul>
            </div>
            <!-- /.navbar-collapse -->
        </div>
    </nav>


    <div class="container"  align="center">
        <img src="figures/puc.png" alt="PUC-Rio">
		<img src="figures/logoopus.png" alt="Opus Research Group">
    </div>

    <div class="container">

        <div class="page-header" id="title" align="center">
            <h1>Graph-based visualization for code smell agglomerations</h1>
            <h2>A controlled experiment</h2>
            <br/>
        </div>

        This web page presents the supplementary material of the paper <i>Graph-based visualization for code smell agglomerations: A controlled experiment</i>. <br>
        

        <br>
        Authors: O.I. Anne Benedicte Agbachi, Leonardo Sousa, Willian Oizumi, Roberto Oliveira, Alessandro Garcia, Anderson Oliveira, Baldoino Fonseca, Carlos Lucena

        <br><br>
        Following sections present the complementary information regarding the paper.

        <h3 class="page-header" id="abstract">Abstract</h3>
		Recent studies indicate that design problems are often related to multiple interrelated code smells. This particular group of code smells can be called a code smell agglomeration. As developers need to analyze agglomerations to identify design problems, a visualization may help them in the analysis. In this context, we conducted a study to evaluate whether a graph-based visualization of agglomerations can help developers to identify design problems. The results show that the visualization can support the design problem identification. Indeed, developers used the visualization to have the first sign of the presence of a design problem. In addition, they used the dependencies presented in the graph to have an overview of complementary symptoms of the same design problem.
        <p class="text-justify">
            . </p>

    </div>
    <!-- /container -->

    <div class="container">

        <h3 class="page-header" id="dp">Design Problems</h3>

        <p class="text-justify">
           
        </p>

        <p class="text-justify">
           

        </p>
        <style type="text/css">
            .tg  {border-collapse:collapse;border-spacing:0;}
            .tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
            .tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
            .tg .tg-xpce{font-weight:bold;background-color:#67fd9a;text-align:center;vertical-align:top}
            .tg .tg-yzt1{background-color:#efefef;vertical-align:top}
        </style>
        <table class="tg" align="center">
            <caption>
                Table I. Design Problem description
            </caption>
            <tr>
                <th class="tg-xpce">Name</th>
                <th class="tg-xpce">Description</th>
            </tr>
            <tr>
                <td class="tg-yzt1">Fat Interface</td>
                <td class="tg-yzt1">Interface of a design component that offers only a general, ambiguous entry-point that provides non-cohesive services, thereby complicating the clients' logic.</td>
            </tr>
            <tr>
                <td class="tg-yzt1">Unwanted Dependency</td>
                <td class="tg-yzt1">Dependency that violates an intended design rule.</td>
            </tr>
            <tr>
                <td class="tg-yzt1">Component Overload</td>
                <td class="tg-yzt1">Design components that fulfill too many responsibilities.</td>
            </tr>
            <tr>
                <td class="tg-yzt1">Cyclic Dependency</td>
                <td class="tg-yzt1">Two or more design components that directly or indirectly depend on each other.</td>
            </tr>
            <tr>
                <td class="tg-yzt1">Delegating Abstraction</td>
                <td class="tg-yzt1">An abstraction that exists only for passing messages from one abstraction to another.</td>
            </tr>
            <tr>
                <td class="tg-yzt1">Scattered Concern</td>
                <td class="tg-yzt1">Multiple components that are responsible for realizing a crosscutting concern.</td>
            </tr>
            <tr>
                <td class="tg-yzt1">Overused Interface</td>
                <td class="tg-yzt1">Interface that is overloaded with many clients accessing it. That is, an interface with "too many clients".</td>
            </tr>
            <tr>
                <td class="tg-yzt1">Unused Abstraction</td>
                <td class="tg-yzt1">Design abstraction that is either unreachable or never used in the system.</td>
            </tr>
        </table>
    </div>

    <div class="container">

        <h3 class="page-header" id="agglomerations">Categories of Agglomeration</h3>

        <p class="text-justify">
           Code smells are recurring micro structures in the source code that may indicate the manifestation of design
            problems <a href="#fowler">(Fowler, 1999)</a>.
        </p>

        <p class="text-justify">
           A code smell agglomeration is a group of inter-related code smells that may indicate the full extension of
            a design problem <a href="#oizumi">(Oizumi, 2016)</a>. The relations among code smells are determined by the relationships that exists between
            the smelly code elements. In our context, a smelly code element is a element that is affected by a code smell.
            Relations among smelly code may assume different forms, according to the agglomeration category. Below, on Table II,
            we present a brief definition of each category
        </p>

        <style type="text/css">
            .tg  {border-collapse:collapse;border-spacing:0;}
            .tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
            .tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
            .tg .tg-kqkn{font-weight:bold;background-color:#67fd9a;text-align:center}
            .tg .tg-bsv2{background-color:#efefef}
        </style>
        <table class="tg" align="center">
            <caption>
                Table II. Agglomeration Categories Definitions
            </caption>
            <tr>
                <th class="tg-kqkn">Category</th>
                <th class="tg-kqkn">Description</th>
            </tr>
            <tr>
                <td class="tg-bsv2">Intra-method</td>
                <td class="tg-bsv2">Agglomerations of code smells that are located in single methods. There is an agglomeration in a method if the method is affected by at least Tmethod + 1 code smells. Tmethod is a threshold that can be defined by the developers.</td>
            </tr>
            <tr>
                <td class="tg-bsv2">Intra-class</td>
                <td class="tg-bsv2">Just like methods, classes may also be affected by diverse code smells. There is an agglomeration in a class if the class is affected by at least Tclass + 1 code smells. Tclass is a threshold that can be defined by the developers.</td>
            </tr>
            <tr>
                <td class="tg-bsv2">Intra-component</td>
                <td class="tg-bsv2">Agglomerations of code smells that occur inside of a single design component. This agglomeration comprises code elements that are located within a single component, and the elements are affected by the same type of code smell. The elements also must be connected by method calls or type references.</td>
            </tr>
            <tr>
                <td class="tg-bsv2">Hierachical</td>
                <td class="tg-bsv2">Agglomerations composed by code elements that are affected by the same type of code smells, and these elements implement the same interface or inherit from the same code element.</td>
            </tr>
        </table>

    </div>

    <div class="container">

        <h3 class="page-header" id="selection">Participant Selection</h3>
        <p class="text-justify">
        

        <p class="text-justify">
            
        </p>

        

        <br>
    </div>

    <div class="container">

        <h3 class="page-header" id="download">Download</h3>

        <p class="text-justify">
            Following we present the main artifacts used in the study. For privacy reasons, we do not provide examples of the videos recorded in the environment, the audio transcription neither the elements affected by design problems.
        </p>

        <table class="tg">
            <caption>
                Table IV. Link to download the artifacts used in the study
            </caption>
            <tr>
                <th class="tg-be9c">Artifact</th>
            </tr>            
            <tr>
                <td class="tg-yzt1"><a href="download/paper.pdf" target="_blank">Submitted Paper</a></td>
            </tr>
            
        </table>

    </div>

    <div class="container">
        <h3 class="page-header" id="references">References</h3>

		<p>
		<ol>
        <li id="shadish">W. R. Shadish, T. D. Cook, and Donald T. Campbell, <i>Experimental and
            Quasi-Experimental Designs for Generalized Causal Inference (2 ed.).</i> Houghton
            Mifflin, 2001</li>
            <li id="trifu">A. Trifu and U. Reupke, <i>Towards automated restructuring of object oriented systems</i> in Proceedings of the 11th European Conference on Software Maintenance and Reengineering, 2007.</li>
            <li id="bar">H. Bär and O. Ciupke, <i>Exploiting design heuristics for automatic problem detection</i> in Workshop Ion on Object-Oriented Technology, 1998.</li>
            <li id="twitter">Twitter. <i>Working at Twitter"</i>. Available at <a href="https://about.twitter.com/careers" target="_blank">https://about.twitter.com/careers</a></li>
            <li id="yahoo">Yahoo!. <i>Explore Career Opportunities"</i>. Available at <a href="https://careers.yahoo.com/us/buildyourcareer" target="_blank">https://careers.yahoo.com/us/buildyourcareer</a></li>
            <li id="fowler">M. Fowler. <i>Refactoring: Improving the Design of Existing Code.</i> Addison-Wesley, Boston, MA, USA, 1999.</li>
            <li id="oizumi">W Oizumi, A Garcia, L Sousa, B Cafeo, and Y Zhao,
                <i>Code Anomalies Flock Together: Exploring Code Anomaly Agglomerations for Locating Design Problems</i>
                in The 38th International Conference on Software Engineering, 2016.ç; USA</li>        
		</ol>
    </div>


</body>

</html>