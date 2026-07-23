VERTUM LANDING PAGE — QUICK START
==================================

1. Unzip this folder anywhere. Keep index.html and the "assets" folder
   together — the page won't find your images if you move one without
   the other.

2. Open index.html by double-clicking it. It already works, using a
   placeholder banner photo so you can see the layout.

3. Add your own photo:
   The only real photograph on the page is the hero banner. Replace:

     assets/garden.jpg   -> big banner photo at the top (~1920x1000px)

   Drag your photo into the /assets folder, rename it to garden.jpg
   (or edit the src="assets/garden.jpg" path in index.html to match
   whatever filename you use), and refresh the page.

4. Your branded artwork is already wired up:

     assets/vertum-vertical-cream.svg  -> hero logo lockup
     assets/plant-icon.svg             -> welcome section icon
     assets/lawn-maint-badge.svg       -> Lawn Maintenance badge
     assets/hedge-pruning-badge.svg    -> Hedge Pruning badge
     assets/plant-care-badge.svg       -> Plant Care badge
     assets/vertum-wordmark.svg        -> nav bar wordmark (drawn inline
                                           in index.html, not loaded as
                                           a separate file — search for
                                           "SITE LOGO MARK" to edit it)
     assets/Vertum-Horizontal-Cream.svg -> spare horizontal lockup,
                                           included but not currently
                                           used anywhere on the page

   To swap any badge or icon for a redesigned version, just overwrite
   the file with the same name and refresh, or open index.html, search
   for the filename (e.g. "lawn-maint-badge.svg") and change the
   src="assets/..." path next to it.

5. Business details: search and replace across index.html:
     "Vertum"                     -> your business name
     "vertum@gmail.com"           -> your email
     "07733234559" / "07733 234559" -> your phone number
     "@vertumgardeningservices"   -> your Instagram handle
   (each detail appears in a couple of places, e.g. the contact section
   and the form's mailto address near the bottom of the file)

6. Colours: near the top of index.html, inside the <style> block, look
   for ":root" — every colour on the page is a variable there. Change
   a value and the whole site updates.

7. Heading font (Bionix): headings use a font called "Bionix" from
   DaFont (https://www.dafont.com/bionix.font). It can't be bundled here
   automatically — download it yourself, check its licence (many DaFont
   fonts are free for personal use only and need a paid licence for
   commercial/business use), then place the font file in:

     assets/fonts/Bionix.woff2   (preferred)
     assets/fonts/Bionix.ttf     (fallback)

   Until you add it, headings will simply display in Josefin Sans —
   nothing will look broken either way.

That's it — no build tools, no dependencies. Just HTML/CSS/JS in one
file, ready to upload to any web host.
