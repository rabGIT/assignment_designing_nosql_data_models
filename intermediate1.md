You're building a restaurant table reserving app that allows users to reserve tables for specified numbers of people. The app will need to show only tables that are available and the times they are available. The app will need to store reservations under a given name with a phone number and number of guests.

tables collection
{
  id: number
  bookings: array of objects
    {
    date:  datetime (only date)
    hours: array of hours, length = hours open
      value = reservation ID if booked for that hour
    }
}

reservations:
{
  ID: number
  name: string
  phone: string: 123-446-7890
  table: id
  date: date of reservation
  time: time of reservation
  guests: number
}
