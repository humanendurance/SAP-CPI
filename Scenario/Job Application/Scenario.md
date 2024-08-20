Working Scenario:
A Candidate is applying for the Job and the information has to be sent in XML Format:

Structure for XML Data:
<profiles> is the root element.
<candidate> is the first child element of <profiles>. The cardinality is 0..n
Each Candidate will have the following Elements:
<firstName> 		: First name of the Candidate 1..1
<lastName> 		: Last Name of the Candidate 0..1
<country>			: Candidate's Country of Residence 1..1
<skills>			: Skills of the Candidate 1..n
Sub Elements of <skills>
<skillName>		: Name of the Skill 1..1
<skillCategory>		: Category of Skill; Allowed Values are Programmer, Software Developer.
<skillProficiency>	: Proficiency of Skill; Allowed Values are Noob, Amateur, Expert, Seasoned

An Example:
<profiles>
	<candidate>
		<firstName>Yeswanth</firstName>
		<lastName>Manikanta</lastName>
		<country>India</country>
		<skills>
			<skillName>C++</skillName>
			<skillCategory>Programmer</skillCategory>
			<skillProficiency>Amateur</skillProficiency>
		</skills>
		<skills>
			<skillName>C</skillName>
			<skillCategory>Software Developer</skillCategory>
			<skillProficiency>Expert</skillProficiency>
		</skills>
	</candidate>
<profiles>

