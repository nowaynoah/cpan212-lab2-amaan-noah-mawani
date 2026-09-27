# Tool Library API

## About
A REST API for a tool library that supports listing, filtering, adding, updating, and deleting tools with validation on every field. 

Live: https://cpan212-lab2-amaan-noah-mawani.onrender.com/api/tools

## Run it

```bash
npm install
cp .env.example .env
npm run dev
```

The API runs at http://localhost:4000. Set `PORT` in `.env` to use a different port.

## Routes

| Method | Path | What it does |
|---|---|---|
| GET | `/api/tools` | Every tool. `?category=garden` keeps only one category |
| GET | `/api/tools/:id` | One tool, or 404 |
| POST | `/api/tools` | Create a tool (201), or 400 with the invalid fields |
| PUT | `/api/tools/:id` | Replace a tool's fields (200), 400 or 404 |
| DELETE | `/api/tools/:id` | Remove a tool (204), or 404 |

## Testing

```bash
npm run check
```

This tries every route and prints which checks pass.

## AI use

Does VSC's built-in IntelliSense count? If so, then really just for any syntax errors I made. Other than that, this was more or less filling in the blanks on code that was already provided in the instructions, so no AI use was needed. 
