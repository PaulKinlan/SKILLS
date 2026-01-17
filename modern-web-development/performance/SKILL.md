---
name: web-performance
description: Expert knowledge in optimizing web application performance for speed, efficiency, and excellent user experience. Covers Core Web Vitals (LCP, FID/INP, CLS), loading optimization, runtime performance, bundle optimization, image optimization, caching strategies, lazy loading, and code splitting. Use when optimizing page load times or improving performance metrics.
metadata:
  version: 1.0.0
---

# Web Performance Skill

Expert knowledge in optimizing web application performance for speed, efficiency, and excellent user experience.

## Core Competencies

- **Core Web Vitals**: Understanding and optimizing LCP, FID/INP, and CLS
- **Loading Performance**: Optimizing page load times and resource delivery
- **Runtime Performance**: Ensuring smooth interactions and animations
- **Bundle Optimization**: Reducing JavaScript bundle sizes
- **Image Optimization**: Using modern formats and responsive images
- **Caching Strategies**: Implementing effective caching mechanisms
- **Lazy Loading**: Deferring non-critical resources
- **Code Splitting**: Breaking up large bundles for faster initial loads

## Key Metrics

- **Largest Contentful Paint (LCP)**: < 2.5s
- **First Input Delay (FID)**: < 100ms
- **Interaction to Next Paint (INP)**: < 200ms
- **Cumulative Layout Shift (CLS)**: < 0.1
- **First Contentful Paint (FCP)**: < 1.8s
- **Time to Interactive (TTI)**: < 3.8s
- **Total Blocking Time (TBT)**: < 200ms

## Optimization Techniques

1. **Resource Loading**
   - Use `async` or `defer` for scripts
   - Preload critical resources
   - Prefetch future navigation resources
   - Use resource hints (dns-prefetch, preconnect)

2. **Image Optimization**
   - Use modern formats (WebP, AVIF)
   - Implement responsive images with srcset
   - Lazy load images below the fold
   - Optimize image compression

3. **JavaScript Optimization**
   - Minimize and compress JavaScript
   - Remove unused code (tree shaking)
   - Code split by route/component
   - Use dynamic imports
   - Avoid long tasks (> 50ms)

4. **CSS Optimization**
   - Minimize critical CSS
   - Remove unused CSS
   - Use CSS containment
   - Optimize animations (use transform and opacity)

5. **Caching**
   - Implement service workers
   - Use appropriate cache headers
   - Version static assets
   - Implement stale-while-revalidate

6. **Network Optimization**
   - Use HTTP/2 or HTTP/3
   - Enable compression (gzip, brotli)
   - Minimize redirects
   - Use CDN for static assets

## Testing Tools

- Lighthouse
- WebPageTest
- Chrome DevTools Performance panel
- Chrome DevTools Coverage panel
- Bundle analyzers (webpack-bundle-analyzer)
- Performance monitoring (Web Vitals library)
