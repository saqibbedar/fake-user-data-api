## Fake User Data API

This repository is a JSON file with fake user data that can be accessed through a simple API. The data includes information about individuals along with their respective categories.

## Access the Data

The JSON data can be accessed using the following URL:

[Raw JSON Data](https://raw.githubusercontent.com/saqibbedar/fake-user-data-api/main/data.json)

## Data Structure

The JSON file follows the structure:

```json
[
    {
        "name": "John",
        "email": "john@fakeEmail.com",
        "category": "Singer"
    },
    // ... (other entries)
]
```

Each entry in the JSON array represents an individual with attributes such as name, email, and category.

## Example Setup

```js
    const fetchData = async ()=>{
        try {
            const response = await fetch("https://raw.githubusercontent.com/saqibbedar/fake-user-data-api/main/data.json");
        if(!response.ok){
            throw new Error("failed to locate resources.");
        }
        const data = await response.json();
        console.log(data);
        }
        catch(error){
            console.error(error);
        }
    };

    fetchData();
```

## Purpose

This repo is for learning purposes, so, feel free to use this fake user data for testing, development, or educational purposes.

## Contribute 😍

Feel free to contribute to this repository by adding more fake data into json file or even adding some additional features. Contributions from the community can make this repository a valuable resource for developers.

Happy coding and learning! 🚀
