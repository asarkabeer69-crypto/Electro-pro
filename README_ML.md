# Electro Master — Android Starter (2D, Malayalam, Offline)

ഇത് Android Studio-യിൽ തുറന്ന് APK ആയി build ചെയ്യാവുന്ന ഒരു starter project ആണ്. 2D wiring practice, Malayalam UI, offline പ്രവർത്തനം എന്നിവയാണ് ലക്ഷ്യം.

## ഉൾപ്പെടുത്തിയിരിക്കുന്നത്
- Android WebView-ൽ പ്രവർത്തിക്കുന്ന offline HTML app
- 2D component selection, terminal-to-terminal virtual wiring
- Main switch / light / fan demo controls
- Fault practice: open circuit, overload, earth leakage, short circuit, open neutral
- Malayalam interface, score and challenges
- Internet permission ഇല്ല

## Build ചെയ്യുന്നത്
1. Android Studio ഇൻസ്റ്റാൾ ചെയ്യുക.
2. `File > Open` വഴി ഈ project folder തുറക്കുക.
3. Gradle sync പൂർത്തിയാകാൻ അനുവദിക്കുക.
4. `Build > Build Bundle(s) / APK(s) > Build APK(s)` തിരഞ്ഞെടുക്കുക.
5. APK സാധാരണയായി `app/build/outputs/apk/debug/app-debug.apk` എന്നിടത്ത് ലഭിക്കും.

## സുരക്ഷാ കുറിപ്പ്
ഇത് വിദ്യാഭ്യാസത്തിനുള്ള simplified training demo മാത്രമാണ്. ഇത് real electrical circuit simulator അല്ല; real 230 V wiring സുരക്ഷിതമാണെന്ന് ഇത് certify ചെയ്യില്ല. യഥാർഥ circuit പരിശോധനയ്ക്ക് approved test instruments, isolation, applicable standards എന്നിവ ആവശ്യമാണ്.

## PC ഇല്ലാതെ APK build ചെയ്യാനുള്ള ഓപ്ഷൻ (GitHub cloud build)
ഈ project-ൽ `.github/workflows/android.yml` ഉൾപ്പെടുത്തിയിട്ടുണ്ട്. ഫോൺ ബ്രൗസറിൽ GitHub അക്കൗണ്ട് തുറന്ന് പുതിയ repository സൃഷ്ടിച്ച് project files upload ചെയ്താൽ GitHub Actions-ൽ cloud build നടത്താം. ശേഷം Actions run-ലെ Artifacts ഭാഗത്ത് നിന്ന് `Electro-Master-debug-APK` ഡൗൺലോഡ് ചെയ്യാം. GitHub UI മാറാം; repository-യിൽ Actions അനുവദിച്ചിരിക്കണം.
