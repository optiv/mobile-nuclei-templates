# Mobile Nuclei Templates

These Nuclei Templates are created to aid mobile security assessments.

Note, the `Keys` folder contain templates to identify API keys based on the regex pattern. So you can run the `Keys` template on a decompiled android app, any local code repository or either 'unzipped' IPA file.

The `Android` folder contain templates specific to Android app. These templates should only run on decompiled Android app as most of the templates are created to perform `smali` checks.

![alt text](https://raw.githubusercontent.com/optiv/mobile-nuclei-templates/main/nuclei-insecureshop.png) 


# How to use?

Make sure to install **Nuclei** from their [Github repo](https://github.com/projectdiscovery/nuclei).

You can now use these templates as follows:

```
echo /output_apktool/ | nuclei -t Keys/xxxxx.yaml
```

If you want to run all the templates at once:

```
echo /output_apktool/ | nuclei -t Keys/
```
