# Data Cleaning and Ranking of User Applications

<p>This project involves the cleaning and ranking of user applications based on specific criteria.</p>

<h3>1. Data Cleaning</h3>
<ul>
  <li>Working with the table from the file <code>applications.csv</code> in Pandas DataFrame</li>
  <li>Duplicates of <code>applicant_id</code> were removed</li>
  <li>Missing values in the 'External Rating' field were filled with zeros</li>
  <li>Missing values in the 'Education level' field were filled with the text “Secondary”</li>
</ul>

<h3>2. Merging Industry Ratings</h3>
<ul>
  <li>Data from the file <code>industries.csv</code> was added to the DataFrame, specifically the industry ratings</li>
</ul>

<h3>3. Application Rating Calculation</h3>
<ul>
  <li>The rating is a number between 0 and 100, based on 6 criteria</li>
  <li>If the 'Amount' is missing or 'External Rating' equals zero, the rating is zero</li>
</ul>

<p><strong>Rating Criteria:</strong></p>
<ul>
  <li>20 points if the applicant's age is between 35 and 55</li>
  <li>20 points if the application was not submitted on a weekend</li>
  <li>20 points if the applicant is married</li>
  <li>10 points if the applicant is located in Kyiv or Kyiv region</li>
  <li>The 'Score' from <code>industries.csv</code> is added (0-20 points)</li>
  <li>20 points if 'External Rating' >= 7</li>
  <li>-20 points if 'External Rating' <= 2</li>
</ul>

<h3>4. Filtering Accepted Applications</h3>
<ul>
  <li>Only applications with a rating greater than zero are accepted</li>
</ul>

<h3>5. Weekly Grouping and Visualization</h3>
<ul>
  <li>Data is grouped by the application submission week, and a graph shows the average rating of accepted applications per week</li>
</ul>

<h3>Tools Used</h3>
<ul>
  <li>Jupyter Notebook</li>
  <li>Python</li>
</ul>
