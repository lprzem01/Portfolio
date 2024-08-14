<h1> Analysis of global marine biodiversity </h1>
<h2>Dataset Overview</h2>
<p>The dataset used for this analysis, titled "Global Marine Biodiversity Data," was obtained from GBIF.org (31 January 2024) through the GBIF Occurrence Download. The dataset includes extensive records on marine species, detailing their occurrences, classifications, and other relevant metadata across various global locations. <a href="https://doi.org/10.15468/dl.uabtae">https://doi.org/10.15468/dl.uabtae</a></p>
<h2>Data preparation</h2>
<p>The dataset was initially loaded and cleaned by replacing missing values with "Unknown" to maintain the integrity of the dataset. The cleaned dataset was structured into a DataFrame with 50 columns, which included information on species identification, taxonomy, location, date, depth, and other attributes relevant to biodiversity studies.</p>

<h2>Biodiversity Analysis</h2>
<p>Biodiversity was analyzed based on various factors such as depth, country, year, and month. The key steps and findings are summarized below:</p>
<ul>
    <li>Color Scheme for Biodiversity Visualization: A predefined color scheme was established using CSS4 color names to ensure a consistent and visually distinct representation of biodiversity across different variables</li>
    <li>Species Count Analysis: Custom functions were implemented to count the number of species per group (e.g., by depth, country, year, and month) and to calculate the number of unique species in each group. Biodiversity was then quantified using a ratio of total species to unique species.</li>
</ul>

<h2>Findings</h2>
<h3>Biodiversity by Depth:</h3>

<p>Species were primarily identified in shallow waters. However, this may be attributed to sampling bias, as shallow areas are more accessible.</p>

<h3>Biodiversity by Country:</h3>

<p>Spain exhibited the highest biodiversity, which could indicate either a genuine biodiversity hotspot or reflect higher sampling efforts in the region.</p>

<h3>Biodiversity by Year:</h3>

<p>A peak in biodiversity was observed around the years 2000-2005. This may correspond to increased sampling efforts or awareness during this period.</p>

<h3>Biodiversity by Month:</h3>

<p>Biodiversity showed a distinct peak in August. Similar to the depth analysis, this peak could be biased if sampling was not conducted uniformly throughout the year.</p>


<div class="graph-container">
    <img src="Biodiversity according to different variables.png" alt="Global Marine Biodiversity">
</div>

<h2>Species and Genus Frequency Analysis</h2>
<p>The most and least common species and genera were identified based on the frequency of occurrences in the dataset. Species like Pelagia noctiluca and genera such as Pinna and Caulerpa were among the most frequently recorded.</p>
<div class="graph-container">
    <img src="Most common species.png" alt="Most Common Species">
</div>


<h2>Statistical Hypothesis Testing</h2>
<p>Two null hypotheses were tested:</p>

<ul>
    <li><strong>H1:</strong> Biodiversity is randomly distributed among countries</li>
    <li><strong>H2:</strong> Pelagia noctiluca is not significantly more common than other species</li>
    <li><strong>H3:</strong> August does not show significantly increased Biodiversity.</li>
</ul>

<ul>
    <li><strong>Biodiversity by country:</strong> Chi-Squared test was performed to determine if biodiversity is randomly distributed among countries, specifically focusing on Spain. The test concluded that biodiversity in Spain is not significantly different from what would be expected by chance, failing to reject the null hypothesis.</li>
    <li><strong>Most common species:</strong>  Chi-Squared test was performed to determine if biodiversity is randomly distributed among countries, specifically focusing on Spain. The test concluded that biodiversity in Spain is not significantly different from what would be expected by chance, failing to reject the null hypothesis.</li>
    <li><strong>Biodiversity by month:</strong> Fail to reject the null hypothesis. August biodiversity is not significantly different than expected by chance..</li>
</ul>
    
<h2>Conclusion</h2>
<p>The analysis provided insights into global marine biodiversity trends based on multiple variables, highlighting areas of potential bias and the need for further investigation, particularly in sampling practices. Spain's high biodiversity and the observed peak in biodiversity during certain periods and locations warrant further research to determine whether these patterns are due to natural factors or methodological biases. Statistical testing revealed no significant anomalies in species distribution, supporting the general findings of the dataset analysis.</p>
