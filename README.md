A static scramjet implementation similar to /staticsj but now uses jsdelivr cdn's to significantly reduce the size of the codebase.

## Proxy configuration and startup
- Default Wisp URL: `wss://wisp.mercurywork.shop`
- The main page now loads Scramjet, then BareMux, then the browser script in order.
- Removed the fake BareMux fallback that could silently start without a real transport.
- The project is still frontend-only: the Wisp endpoint must be online and support the Epoxy transport protocol.
- After replacing files on GitHub Pages, clear this site's data or remove the old `proxServer` localStorage entry if an old endpoint remains selected.
