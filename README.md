# Lin

ORIGIN: https://github.com/questbeat/Lin-Xcode5


## Notes

Added a supported function:
   * LTranslate 

LTranslate is:

    #define LTranslate(key) \
	    [[AppDelegate customLanguageBundle] localizedStringForKey:key value:@"" table:nil]
		
Where customLanguageBundle is dinamically changed in application, when user changes application language

	customLanguageBundle = [NSBundle bundleWithPath:[[NSBundle mainBundle] pathForResource:
        @"en" ofType:@"lproj"]]; 