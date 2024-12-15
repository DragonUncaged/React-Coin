# React-Coin

This project demonstrates how to fetch data from an API, handle the data using React hooks, and display it in a table format. The data is fetched when the component mounts and rendered in a table with separate table row components.

### Features
- Fetch data from a remote API using fetch.
- Manage state with React's useState and trigger data fetching with useEffect.
- Display data dynamically in a table with unique keys for each row.
- Modular approach with a separate TableRow component for displaying each row.

### Technologies Used
- React
- JavaScript (ES6+)
- HTML/CSS

## Key Ponits:
- **Data Fetching**: The useEffect hook triggers the API call once the component is mounted. The fetchData function uses async/await to fetch the data and store it in the data state using setData.
- **State Management**: The fetched data is stored in the state variable data, which is initially an empty array. The setData function updates this state when the API call completes.
- **Rendering and Component Creation**: The TableRow component is used to display each item in the data array. Each object is passed as a prop to the TableRow component for rendering.
- **Mapping and Keys**: The map() method iterates over the data array, rendering each item in a table row. Each row uses a unique key (in this case, item.id) to optimize the rendering performance.
