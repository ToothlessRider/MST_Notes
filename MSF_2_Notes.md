<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MSF_2_Notes</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__left">
    <div class="stackedit__toc">
      
<ul>
<li><a href="#msf-notes-for-mst">MSF Notes for MST</a>
<ul>
<li><a href="#theory-of-automata-">Theory of Automata :</a></li>
<li><a href="#transition-diagram-">Transition Diagram :</a></li>
<li><a href="#transition-table-">Transition Table :</a></li>
<li><a href="#finite-auomata-fa">Finite Auomata FA</a></li>
</ul>
</li>
<li><a href="#deterministic-finite-automata-dfa">Deterministic Finite Automata DFA</a></li>
<li><a href="#non-deterministic-finite-automata-nfa">Non-Deterministic Finite Automata NFA</a></li>
</ul>

    </div>
  </div>
  <div class="stackedit__right">
    <div class="stackedit__html">
      <title>MSF Notes</title>
<h1 id="msf-notes-for-mst">MSF Notes for MST</h1>
<h2 id="theory-of-automata-">Theory of Automata :</h2>
<blockquote>
<p>The study of abstract machines and the computational problems solved using these machines is called the Theory of Automata.</p>
</blockquote>
<h3 id="alphabets-">Alphabets :</h3>
<blockquote>
<p>They are a finite set of symbols. [ Denoted by Σ ]</p>
</blockquote>
<h3 id="string-">String :</h3>
<blockquote>
<p>They are a finite set of symbols, strung together, from the alphabet.</p>
</blockquote>
<h2 id="transition-diagram-">Transition Diagram :</h2>
<p><img src="https://lh7-us.googleusercontent.com/jyQ8o-cdlzV7QpbtxZu-PDr5WOrTjKpfSz4tf9cryX2bwSj4gf7nJnkl5XZxaRBGALxjP0AHpvfPefbetz1_G7MjV3sIoQj-zbHUkqUil9zfgasMcFdE4bn2BJTQCq8WmLDpM9gyPNgHmBog-yV6mIQ" alt=""></p>
<h2 id="transition-table-">Transition Table :</h2>
<p><img src="https://lh7-us.googleusercontent.com/qWA48m8JmeiD-a4dZwwoUjUIeQSOE34-a_zlJb9XXOluX8405rQr_gAXdKRq6QAszygZ5yT1UwCjXGLw31VpD_60_hYqyZN5qa0u9u4WGcab4iILxrGZdXQUtMpo9_3Ymu9kPWkakES_Mski7Hz4SQo" alt=""></p>
<p>==DFA does not have more than a singular entry in each cell</p>
<p>NFA can have multiple entries in each cell==</p>
<h2 id="finite-auomata-fa">Finite Auomata <sub>FA</sub></h2>
<blockquote>
<p>Used to recognize patterns</p>
</blockquote>
<blockquote>
<p>It has two states, i.e. , "Accept State " or " Reject State "</p>
</blockquote>
<p>It is a collection of 5 tuples ( Q, <strong>Σ</strong>, <strong>δ</strong>, q0, F )</p>
<ol>
<li>
<p>Q : Finite set of states</p>
</li>
<li>
<p>Σ : Finite set of input symbols</p>
</li>
<li>
<p>δ : Transition Function</p>
</li>
<li>
<p>q0 : Initial State</p>
</li>
<li>
<p>F : Final State</p>
</li>
</ol>
<h1 id="deterministic-finite-automata-dfa">Deterministic Finite Automata <sub>DFA</sub></h1>
<p>L1 = Set of all strings that start with ‘0’</p>
<ul>
<li>{ 0, 00, 01, 000, 010, 011, 0000, … }</li>
</ul>
<p>Reference Link for DFA video :</p>
<blockquote>
<p><a href="https://www.youtube.com/watch?v=40i4PKpM0cI">DFA by Neso Academy</a></p>
</blockquote>
<p>Q. Construct a DFA that accepts sets of all strings over {0,1} of length 2</p>
<p>Ans.</p>
<p><strong>Σ</strong> = { 0,1 }</p>
<p>L = { 00, 01, 10, 11 }</p>
<pre class=" language-mermaid"><svg id="mermaid-svg-uaDYr60c1WlOW1Hg" width="100%" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" height="124.42500305175781" style="max-width: 425.6625061035156px;" viewBox="0 0 425.6625061035156 124.42500305175781"><style>#mermaid-svg-uaDYr60c1WlOW1Hg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#000000;}#mermaid-svg-uaDYr60c1WlOW1Hg .error-icon{fill:#552222;}#mermaid-svg-uaDYr60c1WlOW1Hg .error-text{fill:#552222;stroke:#552222;}#mermaid-svg-uaDYr60c1WlOW1Hg .edge-thickness-normal{stroke-width:2px;}#mermaid-svg-uaDYr60c1WlOW1Hg .edge-thickness-thick{stroke-width:3.5px;}#mermaid-svg-uaDYr60c1WlOW1Hg .edge-pattern-solid{stroke-dasharray:0;}#mermaid-svg-uaDYr60c1WlOW1Hg .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-svg-uaDYr60c1WlOW1Hg .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-svg-uaDYr60c1WlOW1Hg .marker{fill:#666;stroke:#666;}#mermaid-svg-uaDYr60c1WlOW1Hg .marker.cross{stroke:#666;}#mermaid-svg-uaDYr60c1WlOW1Hg svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#mermaid-svg-uaDYr60c1WlOW1Hg .label{font-family:"trebuchet ms",verdana,arial,sans-serif;color:#000000;}#mermaid-svg-uaDYr60c1WlOW1Hg .cluster-label text{fill:#333;}#mermaid-svg-uaDYr60c1WlOW1Hg .cluster-label span{color:#333;}#mermaid-svg-uaDYr60c1WlOW1Hg .label text,#mermaid-svg-uaDYr60c1WlOW1Hg span{fill:#000000;color:#000000;}#mermaid-svg-uaDYr60c1WlOW1Hg .node rect,#mermaid-svg-uaDYr60c1WlOW1Hg .node circle,#mermaid-svg-uaDYr60c1WlOW1Hg .node ellipse,#mermaid-svg-uaDYr60c1WlOW1Hg .node polygon,#mermaid-svg-uaDYr60c1WlOW1Hg .node path{fill:#eee;stroke:#999;stroke-width:1px;}#mermaid-svg-uaDYr60c1WlOW1Hg .node .label{text-align:center;}#mermaid-svg-uaDYr60c1WlOW1Hg .node.clickable{cursor:pointer;}#mermaid-svg-uaDYr60c1WlOW1Hg .arrowheadPath{fill:#333333;}#mermaid-svg-uaDYr60c1WlOW1Hg .edgePath .path{stroke:#666;stroke-width:1.5px;}#mermaid-svg-uaDYr60c1WlOW1Hg .flowchart-link{stroke:#666;fill:none;}#mermaid-svg-uaDYr60c1WlOW1Hg .edgeLabel{background-color:white;text-align:center;}#mermaid-svg-uaDYr60c1WlOW1Hg .edgeLabel rect{opacity:0.5;background-color:white;fill:white;}#mermaid-svg-uaDYr60c1WlOW1Hg .cluster rect{fill:hsl(210,66.6666666667%,95%);stroke:#26a;stroke-width:1px;}#mermaid-svg-uaDYr60c1WlOW1Hg .cluster text{fill:#333;}#mermaid-svg-uaDYr60c1WlOW1Hg .cluster span{color:#333;}#mermaid-svg-uaDYr60c1WlOW1Hg div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:12px;background:hsl(-160,0%,93.3333333333%);border:1px solid #26a;border-radius:2px;pointer-events:none;z-index:100;}#mermaid-svg-uaDYr60c1WlOW1Hg:root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}#mermaid-svg-uaDYr60c1WlOW1Hg flowchart{fill:apa;}</style><g><g class="output"><g class="clusters"></g><g class="edgePaths"><g class="edgePath LS-A LE-B" style="opacity: 1;" id="L-A-B"><path class="path" d="M54.71250057220459,31.356250762939453L91.04375171661377,31.356250762939453L127.37500286102295,31.356250762939453" marker-end="url(https://stackedit.io/app#arrowhead271)" style="fill:none"></path><defs><marker id="arrowhead271" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath LS-B LE-C" style="opacity: 1;" id="L-B-C"><path class="path" d="M174.08750247955322,31.356250762939453L210.4187536239624,31.356250762939453L246.75000476837158,31.356250762939453" marker-end="url(https://stackedit.io/app#arrowhead272)" style="fill:none"></path><defs><marker id="arrowhead272" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath LS-C LE-D" style="opacity: 1;" id="L-C-D"><path class="path" d="M293.46250438690186,31.356250762939453L332.20625591278076,31.356250762939453L370.95000743865967,31.356250762939453" marker-end="url(https://stackedit.io/app#arrowhead273)" style="fill:none"></path><defs><marker id="arrowhead273" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath LS-D LE-D" style="opacity: 1;" id="L-D-D"><path class="path" d="M385.25969490382727,52.889344244999904L370.95000648498535,86.95000139872232L370.95000648498535,95.0093763669332L394.3062572479248,103.06875133514404L417.66250801086426,95.0093763669332L417.66250801086426,86.95000139872232L403.35281959202234,52.889344244999904" marker-end="url(https://stackedit.io/app#arrowhead274)" style="fill:none"></path><defs><marker id="arrowhead274" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g></g><g class="edgeLabels"><g class="edgeLabel" style="opacity: 1;" transform="translate(91.04375171661377,31.356250762939453)"><g transform="translate(-11.331250190734863,-13.356249809265137)" class="label"><rect rx="0" ry="0" width="22.662500381469727" height="26.712499618530273"></rect><foreignObject width="22.662500381469727" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-A-B" class="edgeLabel L-LS-A' L-LE-B">0,1</span></div></foreignObject></g></g><g class="edgeLabel" style="opacity: 1;" transform="translate(210.4187536239624,31.356250762939453)"><g transform="translate(-11.331250190734863,-13.356249809265137)" class="label"><rect rx="0" ry="0" width="22.662500381469727" height="26.712499618530273"></rect><foreignObject width="22.662500381469727" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-B-C" class="edgeLabel L-LS-B' L-LE-C">0,1</span></div></foreignObject></g></g><g class="edgeLabel" style="opacity: 1;" transform="translate(332.20625591278076,31.356250762939453)"><g transform="translate(-13.74375057220459,-13.356249809265137)" class="label"><rect rx="0" ry="0" width="27.48750114440918" height="26.712499618530273"></rect><foreignObject width="27.48750114440918" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-C-D" class="edgeLabel L-LS-C' L-LE-D">0, 1</span></div></foreignObject></g></g><g class="edgeLabel" style="opacity: 1;" transform="translate(394.3062572479248,103.06875133514404)"><g transform="translate(-11.331250190734863,-13.356249809265137)" class="label"><rect rx="0" ry="0" width="22.662500381469727" height="26.712499618530273"></rect><foreignObject width="22.662500381469727" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-D-D" class="edgeLabel L-LS-D' L-LE-D">0,1</span></div></foreignObject></g></g></g><g class="nodes"><g class="node default" style="opacity: 1;" id="flowchart-A-970" transform="translate(31.356250762939453,31.356250762939453)"><circle x="-14.71875" y="-23.356249809265137" r="23.356249809265137" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-4.71875,-13.356249809265137)"><foreignObject width="9.4375" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">A</div></foreignObject></g></g></g><g class="node default" style="opacity: 1;" id="flowchart-B-971" transform="translate(150.7312526702881,31.356250762939453)"><circle x="-14.53125" y="-23.356249809265137" r="23.356249809265137" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-4.53125,-13.356249809265137)"><foreignObject width="9.0625" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">B</div></foreignObject></g></g></g><g class="node default" style="opacity: 1;" id="flowchart-C-972" transform="translate(270.1062545776367,31.356250762939453)"><circle x="-14.787499904632568" y="-23.356249809265137" r="23.356249809265137" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-4.787499904632568,-13.356249809265137)"><foreignObject width="9.574999809265137" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">C</div></foreignObject></g></g></g><g class="node default" style="opacity: 1;" id="flowchart-D-973" transform="translate(394.3062572479248,31.356250762939453)"><circle x="-14.90625" y="-23.356249809265137" r="23.356249809265137" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-4.90625,-13.356249809265137)"><foreignObject width="9.8125" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">D</div></foreignObject></g></g></g></g></g></g></svg></pre>
<blockquote>
<p>D here is a dead / trap state</p>
</blockquote>
<h1 id="non-deterministic-finite-automata-nfa">Non-Deterministic Finite Automata <sub>NFA</sub></h1>
<pre class=" language-mermaid"><svg id="mermaid-svg-LQHjKQm6oJ25K0V6" width="100%" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" height="62.712501525878906" style="max-width: 383.61248779296875px;" viewBox="0 0 383.61248779296875 62.712501525878906"><style>#mermaid-svg-LQHjKQm6oJ25K0V6{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#000000;}#mermaid-svg-LQHjKQm6oJ25K0V6 .error-icon{fill:#552222;}#mermaid-svg-LQHjKQm6oJ25K0V6 .error-text{fill:#552222;stroke:#552222;}#mermaid-svg-LQHjKQm6oJ25K0V6 .edge-thickness-normal{stroke-width:2px;}#mermaid-svg-LQHjKQm6oJ25K0V6 .edge-thickness-thick{stroke-width:3.5px;}#mermaid-svg-LQHjKQm6oJ25K0V6 .edge-pattern-solid{stroke-dasharray:0;}#mermaid-svg-LQHjKQm6oJ25K0V6 .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-svg-LQHjKQm6oJ25K0V6 .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-svg-LQHjKQm6oJ25K0V6 .marker{fill:#666;stroke:#666;}#mermaid-svg-LQHjKQm6oJ25K0V6 .marker.cross{stroke:#666;}#mermaid-svg-LQHjKQm6oJ25K0V6 svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#mermaid-svg-LQHjKQm6oJ25K0V6 .label{font-family:"trebuchet ms",verdana,arial,sans-serif;color:#000000;}#mermaid-svg-LQHjKQm6oJ25K0V6 .cluster-label text{fill:#333;}#mermaid-svg-LQHjKQm6oJ25K0V6 .cluster-label span{color:#333;}#mermaid-svg-LQHjKQm6oJ25K0V6 .label text,#mermaid-svg-LQHjKQm6oJ25K0V6 span{fill:#000000;color:#000000;}#mermaid-svg-LQHjKQm6oJ25K0V6 .node rect,#mermaid-svg-LQHjKQm6oJ25K0V6 .node circle,#mermaid-svg-LQHjKQm6oJ25K0V6 .node ellipse,#mermaid-svg-LQHjKQm6oJ25K0V6 .node polygon,#mermaid-svg-LQHjKQm6oJ25K0V6 .node path{fill:#eee;stroke:#999;stroke-width:1px;}#mermaid-svg-LQHjKQm6oJ25K0V6 .node .label{text-align:center;}#mermaid-svg-LQHjKQm6oJ25K0V6 .node.clickable{cursor:pointer;}#mermaid-svg-LQHjKQm6oJ25K0V6 .arrowheadPath{fill:#333333;}#mermaid-svg-LQHjKQm6oJ25K0V6 .edgePath .path{stroke:#666;stroke-width:1.5px;}#mermaid-svg-LQHjKQm6oJ25K0V6 .flowchart-link{stroke:#666;fill:none;}#mermaid-svg-LQHjKQm6oJ25K0V6 .edgeLabel{background-color:white;text-align:center;}#mermaid-svg-LQHjKQm6oJ25K0V6 .edgeLabel rect{opacity:0.5;background-color:white;fill:white;}#mermaid-svg-LQHjKQm6oJ25K0V6 .cluster rect{fill:hsl(210,66.6666666667%,95%);stroke:#26a;stroke-width:1px;}#mermaid-svg-LQHjKQm6oJ25K0V6 .cluster text{fill:#333;}#mermaid-svg-LQHjKQm6oJ25K0V6 .cluster span{color:#333;}#mermaid-svg-LQHjKQm6oJ25K0V6 div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:12px;background:hsl(-160,0%,93.3333333333%);border:1px solid #26a;border-radius:2px;pointer-events:none;z-index:100;}#mermaid-svg-LQHjKQm6oJ25K0V6:root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}#mermaid-svg-LQHjKQm6oJ25K0V6 flowchart{fill:apa;}</style><g><g class="output"><g class="clusters"></g><g class="edgePaths"><g class="edgePath LS-A LE-B" style="opacity: 1;" id="L-A-B"><path class="path" d="M54.71250057220459,31.356250762939453L111.58125114440918,31.356250762939453L168.45000171661377,31.356250762939453" marker-end="url(https://stackedit.io/app#arrowhead275)" style="fill:none"></path><defs><marker id="arrowhead275" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath LS-B LE-C" style="opacity: 1;" id="L-B-C"><path class="path" d="M215.16250133514404,31.356250762939453L272.03125190734863,31.356250762939453L328.9000024795532,31.356250762939453" marker-end="url(https://stackedit.io/app#arrowhead276)" style="fill:none"></path><defs><marker id="arrowhead276" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g></g><g class="edgeLabels"><g class="edgeLabel" style="opacity: 1;" transform="translate(111.58125114440918,31.356250762939453)"><g transform="translate(-31.868749618530273,-13.356249809265137)" class="label"><rect rx="0" ry="0" width="63.73749923706055" height="26.712499618530273"></rect><foreignObject width="63.73749923706055" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-A-B" class="edgeLabel L-LS-A' L-LE-B">Link text</span></div></foreignObject></g></g><g class="edgeLabel" style="opacity: 1;" transform="translate(272.03125190734863,31.356250762939453)"><g transform="translate(-31.868749618530273,-13.356249809265137)" class="label"><rect rx="0" ry="0" width="63.73749923706055" height="26.712499618530273"></rect><foreignObject width="63.73749923706055" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-B-C" class="edgeLabel L-LS-B' L-LE-C">Link text</span></div></foreignObject></g></g></g><g class="nodes"><g class="node default" style="opacity: 1;" id="flowchart-A-979" transform="translate(31.356250762939453,31.356250762939453)"><circle x="-14.71875" y="-23.356249809265137" r="23.356249809265137" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-4.71875,-13.356249809265137)"><foreignObject width="9.4375" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">A</div></foreignObject></g></g></g><g class="node default" style="opacity: 1;" id="flowchart-B-980" transform="translate(191.8062515258789,31.356250762939453)"><circle x="-14.53125" y="-23.356249809265137" r="23.356249809265137" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-4.53125,-13.356249809265137)"><foreignObject width="9.0625" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">B</div></foreignObject></g></g></g><g class="node default" style="opacity: 1;" id="flowchart-C-981" transform="translate(352.25625228881836,31.356250762939453)"><circle x="-14.787499904632568" y="-23.356249809265137" r="23.356249809265137" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-4.787499904632568,-13.356249809265137)"><foreignObject width="9.574999809265137" height="26.712499618530273"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">C</div></foreignObject></g></g></g></g></g></g></svg></pre>

    </div>
  </div>
</body>

</html>
