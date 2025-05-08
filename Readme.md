## What are some differences between interfaces and types in TypeScript?
interface is the blueprint of object.An iterface tell the object what kind of properties it's can hold.
And Type is what kind of data it can hold and its used to alis the type.
ex:type username = "string" .now we can assign this value after a variable using colon.
Type gives us more flexibilty then interface .


## What is the use of the keyof keyword in TypeScript? Provide an example.
By using key of we can extract the keys of object type .It ensure the type type safety when accesing the object property dynamically. example

``` interface Person {
  name: string;
  age: number;
  isStudent: boolean;
}

type PersonKeys = keyof Person;
Output: PersonKeys is "name" | "age" | "isStudent"
