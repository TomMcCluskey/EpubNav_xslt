EpubNav_xslt
============

This XSLT is designed to take in an XML file that contains the inforation about a particular epub 3.0 project and return the toc.xhtml, toc.ncx, and content.opf documents. The provided items.xml file shows the format expected by the XSLT. The output is a bit of a hack, honestly; instead of using xsl:result-docment to actually create the new files, the XSLT will produce an html page for display in a web browser like Firefox. From here, the content can be copied and pasted into text files.

To use the xslt, simply edit the items.xml to fit your content and save it. Then open the xml file with Firefox. Firefox will apply the XSLT and display all the navigatoinal documents.

On the Kindle specific documents: This XSLT was originally produced in mid-2012, when Amazon's KindleGen had some non-standard requirements for submitted files. Since then, They have become much better at dealing with standard epub 3.0 files. The three Amazon-specific navigational files are at this point likely vestigal.

On multiple titles and authors: This XSLT does provide support for multiple authors and titles in epub 3.0. However, at present most reading systems do not support this feature, and they all seem to fail in different, creative ways. At present, the best recommendation is to only use epub 2.0.1-style single author and title fields.

To Dos: Add creation of guide, nav landmarks, and pagelist
