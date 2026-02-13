# 3D Web Publish

## Files
- `index.html`
- `crane_scene_web.glb`

## Local preview
```bash
cd /Users/bard/Code/homeBuilder/web/viewer
python3 -m http.server 8080
```
Open `http://localhost:8080`.

## Deploy to Netlify (fastest)
1. Open https://app.netlify.com/drop
2. Drag the folder `/Users/bard/Code/homeBuilder/web/viewer` into the page.
3. Netlify gives you a public URL immediately.

## Deploy to Vercel CLI
```bash
cd /Users/bard/Code/homeBuilder/web/viewer
npx vercel --prod
```

## Notes
- Current GLB size is ~85 MB. For faster web loading, use Draco/mesh simplification before final publish.
- Lighting is material-based in glTF; dynamic shadows depend on viewer/runtime and are not baked lightmaps.
