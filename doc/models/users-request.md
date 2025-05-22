
# Users Request

## Structure

`UsersRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `username` | `?string` | Optional | User's username | getUsername(): ?string | setUsername(?string username): void |
| `age` | `int` | Required | User's age | getAge(): int | setAge(int age): void |
| `isActive` | `?bool` | Optional | Whether the user is active | getIsActive(): ?bool | setIsActive(?bool isActive): void |
| `rating` | `?float` | Optional | User's rating | getRating(): ?float | setRating(?float rating): void |
| `signupDate` | `DateTime` | Required | Signup date | getSignupDate(): \DateTime | setSignupDate(\DateTime signupDate): void |

## Example (as JSON)

```json
{
  "username": "username4",
  "age": 140,
  "isActive": false,
  "rating": 194.34,
  "signupDate": "2016-03-13"
}
```

