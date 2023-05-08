# assigmentDomainModel

Story I - Course Catalog:

Classes:
->siteVisitors
->participants
->course

Attributes:
->siteVisitors:
	->account
	->progress
->participants:
	->userName
	->email
	->password
	->progress
->participants:
	->courseName
	->description
	->endDate
Relations:
->siteVisitors with participants (one to one relationship)
->participants with courses (many to many relationship)

Explanation:

The domain model contains three classes called siteVisitors, participants,
course with each of them having the attributes like above.
the realtion between them is: siteVisitor has a one to one relation with participants
since a participant can only have a account and
participants with course have a many to many realtion
beacuse a participant can have many courses and a course can have many participants. 

Story II - Account Management:

Classes:
->instructor
->courses
->siteVisitors

Attributes:
->instructor:
        ->courseDescription
->courses:
        ->name
        ->description
        ->duration
->siteVisitors:
        ->pages
        ->coursesCatalog
Relations:
->instructor with courses (one to many relationship)
->courses with siteVisitors (many to many relationship)

Explanation:

The domain model contains three classes called instuctor, courses, siteVisitors with each of them 
having the attributes like above.The ralation between them is: 
instuctor with courses have a one to many reation 
because each course can have descriptions that are made by the same instructor
and the relation between courses and siteVisitors is many to many because courses can have only one
description but there are many courses and visitors can view any description for each course.

Story III - Course Creation

Classes:
->instructor
->course 
->participant
->video
->quiz
->discussionForum

Attributes:
->instrutor:
	->name
	->email
->course:
	->name
	->description
	->duration
	->schedule
	->publicationDate
->participant:
	->name 
	->email
->video:
	->name
->quiz:
	->name
->discussionForum:
	->forum
 
Relations:
->instructor with course (one to many realtionship)
->participant with course (one to many relationship)
->video with course (many to one relationship)
->quiz with course (many to one relationship)
->discussionForum with course (optional relationship to optional relationship)

Explanation:

The domain model contains three classes called instuctor, course, participant, video, quiz,
discussion with each of them having the attributes like above.The ralation between them is:
instructor with course has a one to many realtionship because a instucor can manage many courses, 
participant with course has a one to many realtionship because ONE participant can participate in 
many courses ,video with course has a many to one relationship because one course can have many 
videos but those videos can belong to only one course, quiz with course has a many to one relationship 
because one course can have many quzies but those quizes can belong to only one course and 
discussionForum with course have a optional relationship with eachother because a course may or maynot
have a forum. 
