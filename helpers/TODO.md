# TODO List

## Bug Fixes
1. Fix React warning: `ignoreBidiAutoUpdate` prop in RemirrorRenderer component
   - Location: @remirror/react-renderer component
   - Issue: Prop name casing needs to be changed to lowercase

2. Fix React warning: Missing unique "key" props
   - Location: common-widgets package, in list rendering components
   - File: packages/common-widgets/dist/chunk-A37PX364.mjs

3. Address punycode deprecation warning
   - Consider using a userland alternative
   - Affects multiple parts of the application

## Configuration Tasks
1. Set up proper email configuration
   - Configure SMTP settings in .env
   - Test email functionality

2. Set up proper Stripe webhook handling
   - Verify webhook endpoints
   - Test payment processing

## Testing Tasks
1. Test authentication flow
   - Super admin login
   - User registration
   - Password reset

2. Test course creation and management
   - Course creation
   - Content upload
   - Student enrollment

3. Test payment processing
   - Course purchase
   - Subscription handling
   - Refund process

## Performance Optimization
1. Investigate build optimization opportunities
   - Analyze bundle sizes
   - Optimize package dependencies

2. Review and optimize database queries
   - Monitor MongoDB performance
   - Implement caching where necessary

## Internationalization (i18n)
1. Implement Hebrew Translation Support
   - Set up i18n framework
     * Research and implement either next-i18next or react-intl
     * Configure language detection and switching
     * Set up translation file structure

   - Create translation files
     * Set up Hebrew locale files
     * Extract all text content into translation keys
     * Implement RTL (Right-to-Left) support for Hebrew

   - Update Components
     * Modify components to use translation keys
     * Add language switcher component
     * Ensure proper text direction handling

   - Testing Requirements
     * Test language switching functionality
     * Verify RTL layout in Hebrew
     * Test all forms and input fields with Hebrew text

   - Documentation
     * Document translation process for developers
     * Create guidelines for adding new translations
     * Document RTL considerations

2. Quality Assurance
   - Hire professional translator for Hebrew content
   - Set up translation review process
   - Test all features in Hebrew interface

3. Performance Considerations
   - Implement lazy loading for translation files
   - Optimize font loading for Hebrew characters
   - Monitor bundle size impact
