{showThemeSelector Desktop (
<div class="hidden lg:flex">
<ThemeSelectorDropdown class={isFloating ? 'hdr-invert-text' : undefined} />
</div>
)}

{showSearch Desktop (
<div class="flex">
<SearchModal class={isFloating ? 'hdr-invert-text' : undefined} />
</div>
)}

{showThemeSelector Mobile (
<section class="mobile-menu-section">
<p class="mobile-menu-label">{t('nav.sectionTheme', locale)}</p>
<div
class="mobile-menu-stagger flex items-center justify-between rounded-xl px-3 py-2.5"
style={`--stagger-index: ${navItems.length}`}
>
<span class="text-sm text-foreground-muted">{t('theme.colourTheme', locale)}</span>
<ThemeSelector />
</div>
</section>
)}