# merge2pdf - Simplest tool for merging into PDF

Merge Image (jpeg, png) and PDF files (optionally with selective pages) with lossless quality.
It will not convert PDF pages (with texts, images, forms) into flat image, everything will remain as is.

### Install

It's just a single binary file, no external dependencies. 
Just download the executable from Releases page and put it in your (Unix) systems bin directory.
Done! 

### How to use

```bash
# Merge multiple PDFs
merge2pdf output.pdf input1.pdf input2.pdf path/to/other.pdf ...

# Merge 1st page of input1.pdf, full input2.pdf and 2nd, 3rd, 4th page of input3.pdf  
merge2pdf output.pdf input1.pdf~1 input2.pdf input3.pdf~2,3,4
```

If your filename contains space or [some special characters](https://unix.stackexchange.com/a/270979), 
then quote the filepaths along with page numbers. For safety, you can quote them always. 
```bash
merge2pdf output.pdf "With Space.pdf" "without-space.pdf" "with space and pages.pdf~2,3,4"
```

### Roadmap

✅ Merge multiple PDFs without loosing quality  
✅ Merge multiple PDFs with selective pages  
◻️ Adding Images  
◻️ Mixing up Images and PDFs  
◻️ Option to Resize Images to reduce filesize  
◻️ Option to Greyscale Images to reduce filesize  
◻️ Option to set files and pages as JSON config to make usages from other app more convenient  

### Contribute

If you fix a bug or want to add/improve a feature, 
and it's alligned to the focus (merging with ease) of this tool, 
I will be glad to accept your PR.  

### Thanks

This tool was made using the beautiful [Unidoc](https://unidoc.io/) library. Thanks to **Unidoc**.

---
> "This is the Book about which there is no doubt, a guidance for those conscious of Allah" - [Al-Quran](http://quran.com)
