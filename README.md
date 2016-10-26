# XML Converter


Please, keep in mind that XML Converter is a legacy tool, which is only supported for the specific purposes and is not being further developed. We recommend using the proper 3rd party <a href="https://www.microsoft.com/en-us/download/details.aspx?id=21714" target="_blank"><ins><b>Command Line Transformation utility</b></ins></a> to transform source XML into FIDEF format.

This tool is provided for connecting 3rd party systems, or for use in extracting arbitrary metadata from inbound source files.

An example of this is to extract metadata embedded within MXF files, which can then be mapped to the sidecar FIDEF (file definition) XML that will set metadata for input files inside Cinegy.

The tool is expected to be used in a compound script within Cinegy Convert custom pre-execution processing scripts.

## Tool Usage

The package includes the following components: XmlConverter.exe, template.XML, source.XML and output.XML.

where:

* **template.XML** – template of the output file
* **source.XML** – source XML file from which template values are read
* **output.xml** – output file

### How It Works

Converter reads template XML, looks for the special template parameters like “[[ XXX ]]", and these parameters are then replaced with the corresponding values from the source XML.

Please refer to the <a href="https://open.cinegy.com/posts/2016-01-05-xmlconverter/"><b>XML Converter</b></a> post for comprehensive explanation of how to use this tool and view XML samples.