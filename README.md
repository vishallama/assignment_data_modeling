# assignment_data_modeling
Mmmmm.... dataaaaa....

## Authors
Matthew and Vishal


### Basic

1)
#### Goals and Needs:
Keep track of courses and their corresponding lessons. Each course can have
one or more students enrolled in it. And, each student can take one or more
courses.

#### Entities:
Course and Lesson.

#### Attributes:
Course: Key, Id, Title, Description.
Lesson: Key, Id, Title, Body_Text.

#### Types and Constraints
Course: Key(Integer), Id (String), Title (String), Description (Text).
Constraints: Key has to be unique, Id has to be non-empty string, Title
should be less than 255 characters, and Description should be text with at
least 20 chars and no limit.

Lesson: Key(Integer), Id (String), Title (String), Body_Text (Text).
Constraints: Key has to be unique, Id has to be non-empty string, Title
should be less than 255 characters, and Body_Text should be text with at
least 20 chars and no limit.

#### Relationships
A course can have one or more lessons, and a lesson can potentially belong
to more than one course. So, this is a M:N (many to many) relationship.

