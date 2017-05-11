You're building an application that requires user login. Once logged in the user has a bunch of profile information and preference settings available to them. They will need to be able set their birthday, gender, phone number and location (city, state, country). They should be able to provide text to tell about themselves. They also should be able to enable and disable visibility of their birthday, gender, phone number and location.

username: string/only word char
password: string/min 8 char
email: string: word char + '@' + valid domain ending
profile: object
  birthday: date
  gender: string, length 1, M or F
  phone: 123-456-7890
  location: object
    city: string
    state: string
    country: string
  about_me: string
preferences: object
  birthday_visible: true/false
  gender_visible: true/false
  phone_visibile: true/false
  location_visible: true/false
