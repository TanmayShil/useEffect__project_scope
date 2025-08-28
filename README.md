# 🚀 React useEffect Hooks Practice Projects

A collection of React + useEffect practice projects with real-world APIs.
Each mini-project focuses on a specific concept like API fetching, debouncing, pagination, infinite scroll, polling, and device state detection.

---

# 1. Weather App 🌦
API: https://api.openweathermap.org/data/2.5/weather?q={city}&appid={API_KEY} 

Scope:
 - Learn how to fetch dynamic API data using a query parameter (city name).
 - Practice loading state & error handling (Loading..., City not found).
 - Render dynamic UI (temperature, condition, icon).
 - Understand conditional rendering in React.

# 2. GitHub User Finder 🐙
API: https://api.github.com/users/{username} 

Scope:
 - Fetch API data based on user input (username).
 - Handle valid vs invalid user responses (User not found).
 - Display user profile info (name, avatar, bio, followers).
 - Show GitHub repos and link them to external GitHub pages.
 - Learn dependency-based re-fetching → fetch again only when category (repos, followers, etc.) changes.

# 3. News Headlines App 📰
API: https://newsapi.org/v2/top-headlines?country=us&category=${category}&apiKey=${API_KEY} 

Scope:
 - Learn API fetch on component mount (default headlines).
 - Implement dropdown filter (category) → trigger re-fetch.
 - Practice mapping API data into UI (title, description, link).
 - Understand controlled inputs (dropdowns) with useEffect triggers.

# 4. Random Joke Generator 😂
API: https://official-joke-api.appspot.com/random_joke

Scope:
 - Fetch random data on mount.
 - Add a button to re-fetch (new joke on demand).
 - Manage loading & error states.
 - Practice event-based API calls (onClick).

# 5. API Polling (Auto Refresh) ⏳
API: https://api.coindesk.com/v1/bpi/currentprice.json

Scope:
 - Learn polling with setInterval + useEffect.
 - Automatically fetch Bitcoin price every 10s.
 - Understand cleanup function in useEffect (to clear interval).
 - Practice real-time UI updates.

# 6. Debounced Search ⌨️
API: https://jsonplaceholder.typicode.com/posts?title_like=${query} 

Scope:
 - Implement debouncing → wait 500ms before calling API.
 - Prevent excessive API calls while typing.
 - Learn how to use setTimeout and cleanup inside useEffect.
 - Understand optimized API fetching patterns.

# 7. Search with Loading & Error Handling 🔍
API: https://jsonplaceholder.typicode.com/comments?email_like=${query}

Scope:
 - Show loading indicator while fetching.
 - Handle error states (No results, API error).
 - Understand UI states based on API response.
 - Practice search APIs with filters (email_like).

# 8. Paginated Search 📑
API: https://jsonplaceholder.typicode.com/posts?q=${query}&_page=${page}&_limit=10 

Scope:
 - Fetch search results in pages (10 results at a time).
 - Implement pagination (Next/Prev buttons).
 - Learn API query parameters (_page, _limit).
 - Understand state management for page numbers.

# 9. Live Suggestions (AutoComplete) ✍️
API: https://api.datamuse.com/sug?s=${query} 

Scope:
 - Show live word suggestions while typing.
 - Trigger API calls on query change using useEffect.
 - Implement suggestion click → autofill input.
 - Practice real-time search UX like Google.

# 10. Search with Sorting ↕️
API: https://jsonplaceholder.typicode.com/users?name_like=${query} 

Scope:
 - Fetch search results from API.
 - Add sorting feature (by name/id).
 - Learn client-side sorting of fetched data.
 - Practice controlled sorting dropdown + useEffect trigger.

# 11. Search with Infinite Scroll 📜
API: https://jsonplaceholder.typicode.com/posts?q=${query}&_limit=10&_page=${page}

Scope:
 - Fetch search results page by page.
 - Load more data when scroll reaches bottom
 - Practice pagination + infinite scroll mechanism.
 - Handle merging old & new data in state.

# 12. Device & Network State 📱🌐

Scope:
 - Detect online/offline network status with browser events.
 - Display UI feedback (Offline Mode).
 - Learn how to subscribe/unsubscribe to window events inside useEffect.
 - (Optional) Handle device orientation changes (portrait/landscape).
