# CalmSpace

A lightweight, responsive mental wellness support website built with HTML5, CSS, and Vanilla JavaScript.

## Included features

- Responsive single-page navigation for Home, Anxiety, ADHD, Autism, and Contact
- Animated breathing guide with multiple patterns
- Anxiety grounding, color ripple, thought parking, and pulse-counting activities
- ADHD focus timer, memory game, task breakdown, and sequence exercise
- Autism-friendly virtual pop-it, visual rhythm control, and saved comfort plan
- Burnout-prevention prompts and quick check-in suggestions
- Accessibility settings: reduced motion, high contrast, large text, themes, and soft cursor orb toggle
- Local Storage for preferences, exercises, comfort plans, and demo feedback
- Service Worker and web manifest for offline/PWA support
- No framework or build step required

## Run locally

Service workers require HTTP rather than opening the file directly.

### Python

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

### VS Code

Use the Live Server extension and open `index.html`.

## Production notes

- The contact form currently stores feedback locally as a safe demo. Connect it to a secure backend, serverless function, or form provider before launch.
- Add your preferred privacy policy, terms, analytics consent, and region-specific crisis resources.
- The site intentionally avoids autoplay audio and unexpected sensory effects.


## Burnout interaction fix
The pause selector now gives a clear selected state, updates the action button, and initializes independently from the other page tools. The service worker cache was also refreshed to prevent an older JavaScript file from being reused.


## Burnout interaction update
- Tea Ritual replaced with a lightweight interactive Grass Field.
- Sakura petals now react to mouse and touch movement and may be gently guided across the scene.
