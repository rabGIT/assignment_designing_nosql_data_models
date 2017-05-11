You're building a backend for a university that requires students to be able to login. Once logged in, the students can view the exam grades for their classes. They should be able to view results by semester. Each semester should only show the classes in which that student is enrolled that semester.

students
{
  username
  password
  semester: array
    {
      name (of semester): string
      classes: array
        {
          id: string
          name: string
          exams: array of number
          final grade: number
        }
    }
}
