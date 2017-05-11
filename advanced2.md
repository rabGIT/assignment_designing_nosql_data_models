You're building an activity feed for a social media site. The feed must display a chronological list of activities for the current user's friends. These activities could potentially be any action performed on the site including uploading a photo, changing their profile, friending another user, commenting, liking etc... Further, you only want to display activities for users that the current user interacts with frequently.

user collection
{
  user id: number
  user name: string
  friends: array
    {
      friend id: user ID
      friend activity: number (increment when user likes/comments/engaged with friend)
    }
}

activity
{
  user ID: number
  when: datetime
  action: string in {upload photo, change profile, friending, etc.}
  description: string describing activity
}
