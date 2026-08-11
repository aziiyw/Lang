# Roamly

## Turn on real image translation

1. Create a new Vercel project from this folder.
2. In **Project Settings → Environment Variables**, add `GLM_API_KEY` with a newly generated Z.AI key.
3. Deploy. The frontend calls `/api/analyze`; the secret stays on Vercel, never in the browser.

The function uses Z.AI's `glm-5v-turbo` vision model to read the uploaded image, translate it, identify useful travel vocabulary, and return normalized highlight coordinates.
