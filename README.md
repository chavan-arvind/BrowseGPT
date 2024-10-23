# BrowseGPT

[BrowseGPT](https://browsegpt.dev) is a chat interface that allows you to search the web and get answers to your questions. It is built with [Vercel AI SDK](https://www.npmjs.com/package/ai) and [Browserbase](https://www.browserbase.com/).

![BrowseGPT Demo](./app/browsegpt.gif)

## Getting Started

1. Clone the repository
2. Add environment variables (see `.env.template`)
3. Run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

## Using the New Features

### Cloning a Repository

To clone a repository from GitHub, use the `pullRepo` tool. Provide the repository URL and the local path where you want to clone the repository.

Example usage:
```json
{
  "tool": "pullRepo",
  "parameters": {
    "repoUrl": "https://github.com/username/repository.git",
    "localPath": "/path/to/local/directory"
  }
}
```

### Improving Security

To search for the best cyber security practices, use the `improveSecurity` tool. This tool does not require any parameters.

Example usage:
```json
{
  "tool": "improveSecurity",
  "parameters": {}
}
```

## Learn More

To learn more about Vercel AI SDK and Browserbase, take a look at the following resources:

- [Vercel AI SDK](https://www.npmjs.com/package/ai) - learn about Vercel AI SDK features and API.
- [Browserbase](https://www.browserbase.com/) - offers a reliable, high performance serverless developer platform to run, manage, and monitor headless browsers at scale.
