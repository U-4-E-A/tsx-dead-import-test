tsx in watch mode appears to continue to include dead imports.

If the user uncomments the following line in server.ts: -

// import { blah } from "./blah";

... then tsx will now include this and restart if there are any changes in the file.

However, if the import is removed again (commented out) then tsx will continue to watch this file and restart if there are any changes in the file.
