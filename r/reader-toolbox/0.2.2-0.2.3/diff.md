# Comparing `tmp/reader-toolbox-0.2.2.tar.gz` & `tmp/reader-toolbox-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reader-toolbox-0.2.2.tar", last modified: Tue Mar 14 23:10:34 2023, max compression
+gzip compressed data, was "reader-toolbox-0.2.3.tar", last modified: Wed May 31 14:33:38 2023, max compression
```

## Comparing `reader-toolbox-0.2.2.tar` & `reader-toolbox-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-14 23:10:34.367581 reader-toolbox-0.2.2/
--rw-r--r--   0 eric       (501) staff       (20)    18092 2023-03-14 22:36:02.000000 reader-toolbox-0.2.2/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)     3174 2023-03-14 23:10:34.367687 reader-toolbox-0.2.2/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2564 2023-03-14 22:36:02.000000 reader-toolbox-0.2.2/README.md
--rw-r--r--   0 eric       (501) staff       (20)       97 2023-03-14 22:36:03.000000 reader-toolbox-0.2.2/pyproject.toml
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-14 23:10:34.365943 reader-toolbox-0.2.2/rdr/
--rw-r--r--   0 eric       (501) staff       (20)   112978 2023-03-14 23:00:04.000000 reader-toolbox-0.2.2/rdr/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    59032 2023-03-14 22:36:03.000000 reader-toolbox-0.2.2/rdr/rdr.py
--rw-r--r--   0 eric       (501) staff       (20)     4297 2023-03-14 22:36:03.000000 reader-toolbox-0.2.2/rdr/server.py
--rw-r--r--   0 eric       (501) staff       (20)   108746 2023-03-14 22:45:04.000000 reader-toolbox-0.2.2/rdr/x-__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-14 23:10:34.367387 reader-toolbox-0.2.2/reader_toolbox.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     3174 2023-03-14 23:10:34.000000 reader-toolbox-0.2.2/reader_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      340 2023-03-14 23:10:34.000000 reader-toolbox-0.2.2/reader_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-03-14 23:10:34.000000 reader-toolbox-0.2.2/reader_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       36 2023-03-14 23:10:34.000000 reader-toolbox-0.2.2/reader_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 eric       (501) staff       (20)      236 2023-03-14 23:10:34.000000 reader-toolbox-0.2.2/reader_toolbox.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)        4 2023-03-14 23:10:34.000000 reader-toolbox-0.2.2/reader_toolbox.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)      645 2023-03-14 23:10:34.368126 reader-toolbox-0.2.2/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      774 2023-03-14 23:00:04.000000 reader-toolbox-0.2.2/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 14:33:38.191029 reader-toolbox-0.2.3/
+-rw-r--r--   0 eric       (501) staff       (20)    18092 2023-03-14 22:36:02.000000 reader-toolbox-0.2.3/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)     3174 2023-05-31 14:33:38.191115 reader-toolbox-0.2.3/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2564 2023-03-14 22:36:02.000000 reader-toolbox-0.2.3/README.md
+-rw-r--r--   0 eric       (501) staff       (20)       97 2023-03-14 22:36:03.000000 reader-toolbox-0.2.3/pyproject.toml
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 14:33:38.189328 reader-toolbox-0.2.3/rdr/
+-rw-r--r--   0 eric       (501) staff       (20)   128860 2023-05-30 14:35:22.000000 reader-toolbox-0.2.3/rdr/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    60186 2023-05-29 13:29:58.000000 reader-toolbox-0.2.3/rdr/rdr.py
+-rw-r--r--   0 eric       (501) staff       (20)     4297 2023-03-14 22:36:03.000000 reader-toolbox-0.2.3/rdr/server.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 14:33:38.190836 reader-toolbox-0.2.3/reader_toolbox.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     3174 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      322 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       36 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 eric       (501) staff       (20)      236 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)        4 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)      645 2023-05-31 14:33:38.191559 reader-toolbox-0.2.3/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      774 2023-03-14 23:00:04.000000 reader-toolbox-0.2.3/setup.py
```

### Comparing `reader-toolbox-0.2.2/LICENSE` & `reader-toolbox-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reader-toolbox-0.2.2/PKG-INFO` & `reader-toolbox-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reader-toolbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: A command-line interface for creating and interacting with Distant Reader data sets (a.k.a. study carrels)
 Home-page: https://github.com/ericleasemorgan/reader-toolbox
 Author: Eric Lease Morgan
 Author-email: emorgan@nd.edu
 Project-URL: Bug Tracker, https://github.com/ericleasemorgan/reader-toolbox/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `reader-toolbox-0.2.2/README.md` & `reader-toolbox-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `reader-toolbox-0.2.2/rdr/__init__.py` & `reader-toolbox-0.2.3/rdr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,65 +39,84 @@
 REMOTELIBRARY = 'https://distantreader.org'
 CARRELS       = 'stacks/carrels-legacy'
 
 # documentation
 DOCUMENTATION = 'https://reader-toolbox.readthedocs.io'
 
 # file system mappings
-CORPUS               = 'reader.txt'
+AUTHORS              = 'reader.authors'
+BIB                  = 'bib'
+BIBLIOGRAPHYHTML     = 'index.xhtml'
+BIBLIOGRAPHYJSON     = 'bibliography.json'
+BIBLIOGRAPHYTEXT     = 'bibliography.txt'
+BIGRAMSCLOUD         = 'bigrams-cloud.png'
+CACHE                = 'cache'
+CLUSTERCUBE          = 'cluster-cube.png'
+CLUSTERDENDROGRAM    = 'cluster-dendrogram.png'
 COLLOCATIONS         = 'reader.gml'
+CORPUS               = 'reader.txt'
 DATABASE             = 'reader.db'
-VECTORS              = 'reader.vec'
-SENTENCES            = 'reader.sents'
+ENTITIESANY          = 'entities-any.png'
+ENTITIESGPE          = 'entities-gpe.png'
+ENTITIESORG          = 'entities-org.png'
+ENTITIESPERSON       = 'entities-person.png'
 ETC                  = 'etc'
+FIGURES              = 'figures'
 HTM                  = 'htm'
+GML                  = 'reader.gml'
 INDEX                = 'index.htm'
-MANIFEST             = 'MANIFEST.xml'
-STOPWORDS            = 'stopwords.txt'
-LEXICON              = 'lexicon.txt'
-TXT                  = 'txt'
-CACHE                = 'cache'
-PROVENANCE           = 'provenance.tsv'
-METADATA             = 'metadata.csv'
-INDEX                = 'index.htm'
-BIBLIOGRAPHYTEXT     = 'bibliography.txt'
-BIBLIOGRAPHYHTML     = 'bibliography.htm'
-BIBLIOGRAPHYJSON     = 'bibliography.json'
-SIZESBOXPLOT         = 'sizes-boxplot.png'
-SIZESHISTOGRAM       = 'sizes-histogram.png'
-READABILITYHISTOGRAM = 'readability-histogram.png'
-READABILITYBOXPLOT   = 'readability-boxplot.png'
-CLUSTERDENDROGRAM    = 'cluster-dendrogram.png'
-CLUSTERCUBE          = 'cluster-cube.png'
-FIGURES              = 'figures'
+INDEXRDF                  = 'index.rdf'
 KEYWORDSCLOUD        = 'keywords-cloud.png'
-UNIGRAMSCLOUD        = 'unigrams-cloud.png'
-BIGRAMSCLOUD         = 'bigrams-cloud.png'
-ENTITIESANY          = 'entities-any.png'
-ENTITIESPERSON       = 'entities-person.png'
-ENTITIESGPE          = 'entities-gpe.png'
-ENTITIESORG          = 'entities-org.png'
-POSNOUN              = 'pos-noun.png'
-POSVERB              = 'pos-verb.png'
-POSPRON              = 'pos-pronoun.png'
+LEXICON              = 'lexicon.txt'
+MANIFEST             = 'MANIFEST.xml'
+METADATA             = 'index.csv'
 POSADJ               = 'pos-adjective.png'
 POSADV               = 'pos-adverb.png'
+POSNOUN              = 'pos-noun.png'
+POSPRON              = 'pos-pronoun.png'
 POSPROPN             = 'pos-propernoun.png'
+POSVERB              = 'pos-verb.png'
+PROVENANCE           = 'index.tsv'
+READABILITYBOXPLOT   = 'readability-boxplot.png'
+READABILITYHISTOGRAM = 'readability-histogram.png'
+SENTENCES            = 'reader.sents'
+SIZESBOXPLOT         = 'sizes-boxplot.png'
+SIZESHISTOGRAM       = 'sizes-histogram.png'
+STOPWORDS            = 'stopwords.txt'
+TXT                  = 'txt'
+UNIGRAMSCLOUD        = 'unigrams-cloud.png'
+VECTORS              = 'reader.vec'
+WRD                  = 'wrd'
+WRDS                 = 'reader.wrds'
+ZIP                  = 'index.zip'
 
 # spacy langauge model
 MODELSMALL   = 'en_core_web_sm'
-MODELMEDIUM  = 'en_core_web_md'
+MODELMEDIUM  = 'en_core_web_sm'
 
 # mallet
 MALLETZIP = 'https://distantreader.org/apps/mallet.zip'
 MALLETBIN = 'bin/mallet'
 
 # tika server
 TIKADOWNLOAD = 'https://distantreader.org/apps/tika-server.jar'
 
+# xhtml template for bibliography (index.xhtml)
+XHTML = '''
+<!DOCTYPE html>
+<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en">
+<head><title>Bibliography</title></head>
+<body style="margin:3%">
+<h1>Bibliography</h1>
+<p>This is an automatically generated bibliography describing the content of this study carrel.</p>
+<ol>##ITEMS##</ol>
+</body>
+</html>
+'''
+
 # html template for summarize command
 TEMPLATE = '''
 <html>
 <head>
 <title>Index of ##CARREL##</title>
 </head>
 <body style='margin: 7%'>
@@ -264,14 +283,445 @@
 	# iterate
 	def __iter__( self ) :
 			
 		# return each sentence
 		for sentence in open( self.file ) : yield sentence
 
 
+# return the object of a given subject/predicate pair
+def rdfSearchForObject ( graph, subject, predicate ) :
+	sparql = 'SELECT ?object WHERE {<' + str( subject ) + '> <' + predicate + '> ?object}'
+	object = graph.query( sparql ).bindings[ 0 ][ 'object' ]
+	return object
+	
+
+# return the English label of a given object
+def rdfSearchForLabel ( graph, object ) :
+	sparql = 'SELECT ?label WHERE {<' + str( object ) + '> rdfs:label ?label . FILTER(LANG(?label) = "en")}'
+	label  = graph.query( sparql ).bindings[ 0 ][ 'label' ]
+	return label
+
+	
+# given the name of a carrel, return GML
+def graph2gml( carrel, output='gml', save=False, erase=False ) :
+
+	'''Given the name of a carrel, and an optional output type ('gml' or 'chart'), return GML or its visualization.'''
+	
+	# configure
+	FORMAT  = 'xml'
+	CARREL  = 'https://distantreader.org/carrel#'
+	WDP     = 'http://www.wikidata.org/prop/direct/'
+	DCTITLE = 'http://purl.org/dc/terms/title'
+	OUTPUTS = [ 'gml', 'chart' ]
+	
+	# require
+	from rdflib.namespace import DCTERMS, RDFS
+	import networkx
+	import rdflib
+	import sys
+	
+	# sanity check #0
+	if output not in OUTPUTS :
+	
+		click.echo( "Error: Unsupported value for output (" + str( output ) + "); exiting.", err=True )
+		exit()
+		
+	# sanity check #1
+	checkForCarrel( carrel )
+	
+	# initialize
+	graph   = rdflib.Graph()
+	library = configuration( 'localLibrary' )
+
+	# sanity check #2
+	authors  = library/carrel/ETC/AUTHORS
+	keywords = library/carrel/ETC/WRDS
+	if not authors.exists()  : reconcile( carrel, 'authors' )
+	if not keywords.exists() : reconcile( carrel, 'keywords' )
+
+	# more configuration and santity checks
+	rdf = library/carrel/INDEXRDF
+	if not rdf.exists() : carrel2graph( carrel )
+
+	# yet more initialization
+	graph  = graph.parse( rdf, format=FORMAT )
+	CARREL = rdflib.Namespace( CARREL )
+	WDP    = rdflib.Namespace( WDP )
+	nodes  = []
+	edges  = []
+
+	# process all keywords
+	for subject, predicate, object in graph.triples( ( None, CARREL.keyword, None ) ) :
+	
+		# get the subject's corresponding title
+		subject = rdfSearchForObject( graph, subject, DCTITLE )
+		
+		# update
+		nodes.append( ( subject, { 'types' : 'item' } ) )
+		nodes.append( ( object, { 'types' : 'keyword' } ) )
+		edges.append( ( subject, object, { 'types' : 'keyword' } ) )
+
+	# process all subjects
+	for subject, predicate, object in graph.triples( ( None, DCTERMS.subject, None ) ) :
+							
+		# get the subject's title and the object's label
+		subject = rdfSearchForObject( graph, subject, DCTITLE )
+		object  = rdfSearchForLabel( graph, object )
+					
+		# update
+		nodes.append( ( subject, { 'types' : 'item' } ) )
+		nodes.append( ( object, { 'types' : 'subject' } ) )
+		edges.append( ( subject, object, { 'types' : 'subject' } ) )
+
+	# process all authors
+	for subject, predicate, object in graph.triples( ( None, CARREL.hasAuthor, None ) ) :
+	
+		# get the subject's corresponding title
+		subject = rdfSearchForObject( graph, subject, DCTITLE )
+
+		# update 
+		nodes.append( ( subject, { 'types' : 'item' } ) )
+		nodes.append( ( object, { 'types' : 'author' } ) )
+		edges.append( ( subject, object, { 'types' : 'author' } ) )
+
+	# process all creators
+	for subject, predicate, object in graph.triples( ( None, DCTERMS.creator, None ) ) :
+	
+		# get the subject's corresponding title
+		subject = rdfSearchForObject( graph, subject, DCTITLE )
+		object  = rdfSearchForLabel( graph, object )
+
+		# update 
+		nodes.append( ( subject, { 'types' : 'item' } ) )
+		nodes.append( ( object, { 'types' : 'creator' } ) )
+		edges.append( ( subject, object, { 'types' : 'creator' } ) )
+
+	# build the graph; very smart
+	graph = networkx.Graph()
+	graph.add_nodes_from( nodes )
+	graph.add_edges_from( edges )
+
+	# GML output
+	if output == 'gml' :
+	
+		# save
+		if save == True :
+		
+			gml = library/carrel/ETC/GML
+			networkx.write_gml( graph, gml )
+
+		# send to STDOUT
+		else : networkx.write_gml( graph, sys.stdout.buffer )
+
+	# chart output
+	if output == 'chart' : click.echo( "Warning: The output value of chart is not implemented, yet.", err=True )
+
+
+# given the name of a carrel, create an RDF file describing it
+def carrel2graph( carrel ) :
+
+	'''Given the name of a carrel, create an RDF file (index.rdr) describing it.'''
+	
+	# configure
+	NAMESPACE = 'https://distantreader.org/carrel#'
+	PREFIX    = 'carrel'
+	FORMAT    = 'xml'
+	GRAPHROOT = 'http://distantreader.org/stacks/carrels/'
+	CREATOR   = { 'name':"Eric Lease Morgan", 'qnumber':'https://www.wikidata.org/wiki/Q102275801' }
+	TEMPLATE  = '''PREFIX wd: <http://www.wikidata.org/entity/> CONSTRUCT { wd:##QNUMBER## ?p ?o } WHERE { SERVICE <https://query.wikidata.org/bigdata/namespace/wdq/sparql> { wd:##QNUMBER## ?p ?o }}'''
+	WIKIDATA  = 'http://www.wikidata.org/entity/'
+
+	# require
+	from rdflib           import Graph, URIRef, Literal, Namespace
+	from rdflib.namespace import RDF, DCTERMS, DCMITYPE, RDFS
+	import pandas as pd
+	import json
+
+	# sanity check
+	checkForCarrel( carrel )
+	
+	# initialize
+	studyCarrel = carrel
+	graph       = Graph()
+	CARREL      = Namespace( NAMESPACE )
+	library     = configuration( 'localLibrary' )
+	graph.bind( PREFIX, CARREL )
+
+	# denote a carrel and update the graph
+	carrel  = URIRef( GRAPHROOT + studyCarrel )
+	graph.add( ( carrel, RDF.type,        CARREL.carrel ) )
+	graph.add( ( carrel, RDF.type,        DCMITYPE.Dataset ) )
+	graph.add( ( carrel, RDF.type,        DCMITYPE.Collection ) )
+	graph.add( ( carrel, DCTERMS.title,   Literal( studyCarrel ) ) )
+
+	# add the carrel's creator (me)
+	#qnumber = URIRef( CREATOR[ 'qnumber' ] )
+	#graph.add( ( carrel, DCTERMS.creator, qnumber ) )
+	#graph.add( ( qnumber, RDFS.label,     Literal( CREATOR[ 'name' ] ) ) )
+
+	# get provenance and extents...
+	dateCreated      = provenance( studyCarrel, 'dateCreated' )
+	process          = provenance( studyCarrel, 'process' )
+	totalSizeInItems = extents( studyCarrel,    'items' )
+	totalSizeInWords = extents( studyCarrel,    'words' )
+	averageFlesch    = extents( studyCarrel,    'flesch' )
+
+	# ...and update the graph
+	graph.add( ( carrel, DCTERMS.created,            Literal( dateCreated ) ) )
+	graph.add( ( carrel, CARREL.hasCreationProcess,  Literal( process ) ) )
+	graph.add( ( carrel, CARREL.hasTotalSizeInItems, Literal( totalSizeInItems ) ) )
+	graph.add( ( carrel, CARREL.hasTotalSizeInWords, Literal( totalSizeInWords ) ) )
+	graph.add( ( carrel, CARREL.hasAverageFlesch,    Literal( averageFlesch ) ) )
+
+	# get the name of the keywords reconciliation file, and check
+	keywords = library/studyCarrel/ETC/WRDS
+	if not keywords.exists() :
+	
+		click.echo( "The keywords reconciliation file does not exist. Please create one. Exiting.", err=True )
+		exit()
+		
+	# reconciliation file exists
+	else :
+	
+		# get and process all keyword qunumbers; update the graph with reconciled values
+		keywords = pd.read_csv( keywords, sep='\t', dtype={'id': str} )
+		qnumbers = set( keywords[ keywords[ 'qnumber' ].notnull() ][ 'qnumber' ].tolist() )
+
+	# get wikidata qnumbers, if they exist
+	qnumbers = sorted( qnumbers)
+	length   = len( qnumbers )
+	for index, qnumber in enumerate( qnumbers ) :
+
+		# debug, create SPARQL query, search, get result, and update graph
+		click.echo( "Getting Wikidata for keyword " + qnumber + ' (#' + str( index + 1 ) + ' of ' + str( length) + ')', err=True )
+		sparql = TEMPLATE.replace( '##QNUMBER##', qnumber )
+		rdf    = graph.query( sparql ).serialize( format=FORMAT )
+		graph.parse( rdf, format=FORMAT )	
+
+	# get the name of the authors reconciliation file, and check
+	authors = library/studyCarrel/ETC/AUTHORS
+	if not authors.exists() :
+	
+		click.echo( "The authors reconciliation file does not exist. Please create one. Exiting.", err=True )
+		exit()
+
+	# reconciliation file exists
+	else :
+	
+		# get and process all author qunumbers; update the graph with reconciled values
+		authors  = pd.read_csv( authors, sep='\t' )
+		qnumbers = set( authors[ authors[ 'qnumber' ].notnull() ][ 'qnumber' ].tolist() ) 
+
+	# process all author qunumbers; update the graph with reconciled values some more
+	qnumbers = sorted( qnumbers)
+	length   = len( qnumbers )
+	for index, qnumber in enumerate( qnumbers ) :
+
+		# debug, create SPARQL query, search, get result, and update graph
+		click.echo( "Getting Wikidata for author " + qnumber + ' (#' + str( index + 1 ) + ' of ' + str( length) + ')', err=True )
+		sparql = TEMPLATE.replace( '##QNUMBER##', qnumber )
+		rdf    = graph.query( sparql ).serialize( format=FORMAT )
+		graph.parse( rdf, format=FORMAT )	
+
+	# get and process each bibliographic item
+	bibliographics = json.loads( bibliography( studyCarrel, format='json' ) )
+	length         = len( bibliographics )
+	for index, bibliographic in enumerate( bibliographics ) :
+		
+		# debug
+		click.echo( 'Adding item ' + str( index ) + ' of ' + str( length ) + '\r', nl=False, err=True )
+	
+		# get the item's id and update the graph
+		idItem = str( bibliographic[ 'id' ] )
+		item   = URIRef( idItem )
+		graph.add( ( carrel, DCTERMS.hasPart, item ) )
+	
+		# process authors, conditionally
+		if not authors.empty :
+	
+			# iterate over the keywords
+			for _, author in authors.iterrows() :
+			
+				# update the graph, conditionally
+				if str( author[ 'id' ] ) == idItem :
+				
+					# get the qnumber and update the graph, conditionally
+					qnumber = author[ 'qnumber' ]
+					if type( qnumber ) is str : graph.add( ( item, DCTERMS.creator, URIRef( WIKIDATA + qnumber ) ) )
+					else : graph.add( ( item, CARREL.hasAuthor, Literal( author[ 'author' ] ) ) )
+
+		# add title
+		graph.add( ( item, DCTERMS.title, Literal( bibliographic[ 'title' ] ) ) )
+
+		# add date
+		graph.add( ( item, DCTERMS.date, Literal( bibliographic[ 'date' ] ) ) )
+
+		# add extents; using try is a hack for bogus data
+		try : graph.add( ( item, CARREL.hasFlesch, Literal( int( bibliographic[ 'flesch' ] ) ) ) )
+		except TypeError : continue
+		graph.add( ( item, CARREL.hasSizeInWords, Literal( int( bibliographic[ 'words' ] ) ) ) )
+
+		# add cache and plain text	
+		cache = URIRef( GRAPHROOT + studyCarrel + '/' + ( CACHE ) + '/' + idItem + bibliographic[ 'extension' ] )
+		text  = URIRef( GRAPHROOT + studyCarrel + '/' + ( TXT )   + '/' + idItem + '.txt' )
+		graph.add( ( item,  CARREL.hasCache,     cache ) )
+		graph.add( ( item,  CARREL.hasPlainText, text ) )
+		graph.add( ( cache, DCTERMS.type,        Literal( bibliographic[ 'mime' ] ) ) )
+		graph.add( ( text,  DCTERMS.type,        Literal( 'text/plain' ) ) )
+	
+		# process keywords, conditionally
+		if not keywords.empty :
+			
+			# iterate over the keywords
+			for _, keyword in keywords.iterrows() :
+						
+				# update the graph, conditionally
+				if str( keyword[ 'id' ] ) == idItem :
+				
+				
+					# get the qnumber and update the graph, conditionally
+					qnumber = keyword[ 'qnumber' ]
+					if type( qnumber ) is str : graph.add( ( item, DCTERMS.subject, URIRef( WIKIDATA + qnumber ) ) )
+					else : graph.add( ( item, CARREL.keyword, Literal( keyword[ 'keyword' ] ) ) )
+
+	# output and done
+	rdf = library/studyCarrel/INDEXRDF
+	with open( rdf, 'w' ) as handle : handle.write( graph.serialize( format=FORMAT ) )
+
+
+# given a carrel and a type, (re-)create reconciliation file(s)
+def reconcile( carrel, type, erase=False ) :
+
+	'''Given the name of a carrel and a type ('author' or 'keyword'), (re-)initialize a recoconciliation file'''
+
+	# configure
+	PATTERN  = '*'
+	AUTHORS  = [ 'id', 'author', 'qnumber' ]
+	KEYWORDS = [ 'id', 'keyword', 'qnumber' ]
+	TYPES    = [ 'authors', 'keywords' ]
+	
+	# require
+	from   glob import glob
+	import pandas as pd
+	import rdr
+	import sys
+
+	# sanity check #1
+	rdr.checkForCarrel( carrel )
+
+	# sanity check #2
+	if type not in TYPES :
+	
+		click.echo( "Error: Unknown value for type (" + str( type ) + "); exiting", err=True )
+		exit()
+	
+	# debug
+	click.echo( 'Reconciling ' + type + " of " + carrel, err=True )
+
+	# initialize
+	library  = rdr.configuration( 'localLibrary' )
+	authors  = library/carrel/( rdr.ETC )/( rdr.AUTHORS )
+	keywords = library/carrel/( rdr.ETC )/( rdr.WRDS )
+
+	# check whether or not we've already been here, and get files to reconcile, conditionally
+	if type == 'authors' :
+			
+		# check to see if the file ought to be overwritten
+		if authors.exists() and erase == False :
+	
+			click.echo( "Warning: Authors reconciliation exists and erase is false, thus, not overwriting; exiting.\n", err=True )
+			exit()
+	
+		# delete the existing reconcilation
+		else: authors.unlink( missing_ok=True )
+
+		# get the files to process
+		files = glob( str( library/carrel/( rdr.BIB )/PATTERN ) )
+
+	# check whether or we've already been here, and get files to reconcile, conditionally
+	if type == 'keywords' :
+			
+		# check to see if the file ought to be overwritten
+		if keywords.exists() and erase == False :
+	
+			click.echo( "Warning: Keywords reconciliation exists and erase is false, thus, not overwriting; exiting.\n", err=True )
+			exit()
+	
+		# delete the existing reconcilation
+		else: keywords.unlink( missing_ok=True )
+
+		# get the files to process
+		files   = glob( str( library/carrel/( rdr.WRD )/PATTERN ) )
+
+	# create a dataframe of all records and process each; reconcile
+	reconciliations = []
+	records         = pd.concat( ( pd.read_csv( file, sep='\t', dtype={ 'id': str } ) for file in files ) )
+	for index, record in records.iterrows() :
+	
+		# reconcile; here is where we add qnumbers from a dictionary
+		if type == 'authors'  : reconciliation = [ record[ 'id' ], record[ 'author' ], '' ]
+		if type == 'keywords' : reconciliation = [ record[ 'id' ], record[ 'keyword' ], '' ]
+		
+		# update
+		reconciliations.append( reconciliation )
+		
+	# create a dataframe of reconciliations, output, and done
+	if type == 'authors' :
+		reconciliations = pd.DataFrame( reconciliations, columns=AUTHORS )
+		with open( authors, 'w' ) as handle : handle.write( reconciliations.to_csv( sep='\t', index=False ) )
+
+	if type == 'keywords' :
+		reconciliations = pd.DataFrame( reconciliations, columns=KEYWORDS )
+		with open( keywords, 'w' ) as handle : handle.write( reconciliations.to_csv( sep='\t', index=False ) )
+
+
+# given the name of a carrel, create zip file (index.zip) in its root
+def carrel2zip( carrel ) :
+
+	'''Given then name of a carrel, create a zip file (index.zip)
+	in its root.'''
+
+	# I don't know were to require these, here or at the root?
+	from zipfile import ZipFile
+	import os
+	import tempfile
+	import shutil
+	
+	# sanity check
+	rdr.checkForCarrel( carrel )
+	
+	# initialize
+	library = configuration( 'localLibrary' )
+	zip     = library/carrel/ZIP
+	staging = tempfile.NamedTemporaryFile( delete=False ).name
+	
+	# debug
+	click.echo( "Creating archive (index.zip) file of " + carrel, err=True )
+	
+	# make sane
+	zip.unlink( missing_ok=True )
+	os.chdir( library )
+	
+	# create an archive
+	with ZipFile( staging, 'w' ) as handle :
+
+		# find all files
+		for root, _, files in os.walk( carrel ) :
+
+			# process each file
+			for file in files:
+			
+				# create full path name, debug, and do the work
+				file = os.path.join( root, file )
+				click.echo( file, err=True )
+				handle.write( file )
+
+	# put the archive into place
+	shutil.move( staging, zip )
+
 # given a sentence, parser, and lexicon return matching sentences
 def matchModal( sentence, parser, lexicon ) :
 		
 	'''Given a sentence, an NLTK RegexpParser object (a grammar), and a
 	lexicon (a set of strings), return the sentence if it matches the
 	object's grammar, otherwise return None.'''
 	
@@ -622,15 +1072,15 @@
 
 	# initialize
 	locallibrary           = configuration( 'localLibrary' )
 	connection             = sqlite3.connect( str( locallibrary/carrel/ETC/DATABASE )  )
 	connection.row_factory = sqlite3.Row
 
 	# query database
-	sql  = '''SELECT b.id, b.words, b.extension, b.flesch, b.author, b.title, b.date, GROUP_CONCAT( LOWER( w.keyword ), '; ') AS keywords, b.summary
+	sql  = '''SELECT b.id, b.words, b.extension, b.flesch, b.author, b.title, b.date, GROUP_CONCAT( LOWER( w.keyword ), '; ') AS keywords, b.summary, b.mime
 			  FROM bib AS b, wrd AS w
 			  WHERE b.id = w.id
 			  GROUP BY b.id
 			  ORDER BY b.id, LOWER( b.author );'''
 	rows  = connection.execute( sql )
 	rows  = rows.fetchall()
 	connection.close()
@@ -640,15 +1090,15 @@
 		
 	elif format == 'text' or format == 'html' :
 	
 		# initialize
 		total        = len( rows )
 		bibliography = ''
 		items        = ''
-		template     = "<html><head><title>Bibliography</title></head><body style='margin:7%'><h1>Bibliography</h1><ol>##ITEMS##</ol></body></html>"
+		template     = XHTML
 		
 		# process each row
 		for item, row in enumerate( rows ) :
 
 			# parse
 			id        = str( row[ 'id' ] )
 			author    = row[ 'author' ]
@@ -663,19 +1113,22 @@
 			if summary : summary = summary.replace( "''", "'" )
 	
 			# a hack for the lack of an extension
 			if not row[ 'extension' ] : extension = ''
 			else                      : extension = row[ 'extension' ]
 			
 			# build cache and plain text
-			cache = str( locallibrary/carrel/CACHE/id ) + extension
-			text  = str( locallibrary/carrel/TXT/id )   + '.txt'
+			#cache = str( locallibrary/carrel/CACHE/id ) + extension
+			#text  = str( locallibrary/carrel/TXT/id )   + '.txt'
 	
 			if format == 'text' :
 			
+				cache = str( locallibrary/carrel/CACHE/id ) + extension
+				text  = str( locallibrary/carrel/TXT/id )   + '.txt'
+				
 				# build the bibliography
 				bibliography = bibliography + ( '        item: #%s of %s\n' % ( str( item + 1 ), total ) )
 				bibliography = bibliography + ( '          id: %s\n' % id )
 				bibliography = bibliography + ( '      author: %s\n' % author )
 				bibliography = bibliography + ( '       title: %s\n' % title )
 				bibliography = bibliography + ( '        date: %s\n' % date )
 				bibliography = bibliography + ( '       words: %s\n' % words )
@@ -684,34 +1137,36 @@
 				bibliography = bibliography + ( '    keywords: %s\n' % keywords )
 				bibliography = bibliography + ( '       cache: %s\n' % cache )
 				bibliography = bibliography + ( '  plain text: %s\n' % text )
 				bibliography = bibliography + '\n'
 	
 			else :
 			
+				cache = './' + CACHE + '/' + id + extension
+				text  = './' + TXT + '/' + id + '.txt'
+				
 				item = '<ul>'
 				item = item + '<li>' + ( 'author: %s'    % author )   + '</li>'
 				item = item + '<li>' + ( 'title: %s'     % title )    + '</li>'
 				item = item + '<li>' + ( 'date: %s'      % date )     + '</li>'
 				item = item + '<li>' + ( 'words: %s'     % words )    + '</li>'
 				item = item + '<li>' + ( 'flesch: %s'    % flesch )   + '</li>'
 				item = item + '<li>' + ( 'summary: %s'   % summary )  + '</li>'
 				item = item + '<li>' + ( 'keywords: %s'  % keywords ) + '</li>'
-				item = item + '<li>' + ( 'cache: %s'      % cache )   + '</li>'
-				item = item + '<li>' + ( 'plain text: %s' % text )    + '</li>'
+				item = item + '<li>' + ( 'versions: <a href="' + cache + '">original</a>; <a href="' + text + '">plain text</a>' ) + '</li>'
 				item = item + '</ul>'
 				
 				items = items + "<li>" + id + item + "</li>"
 				
 	if format == 'html' : bibliography = template.replace( '##ITEMS##', items )
 	
 	if save :
 
 		if format == 'text' : file = locallibrary/carrel/ETC/BIBLIOGRAPHYTEXT
-		if format == 'html' : file = locallibrary/carrel/ETC/BIBLIOGRAPHYHTML
+		if format == 'html' : file = locallibrary/carrel/BIBLIOGRAPHYHTML
 		if format == 'json' : file = locallibrary/carrel/ETC/BIBLIOGRAPHYJSON
 		
 		with open( file, 'w', encoding='utf-8' ) as handle : handle.write( bibliography )
 		
 	else : return bibliography
 	
 
@@ -1079,16 +1534,19 @@
 			
 		# create a simple list of words, and store it in a dataframe
 		records = []
 		for row in rows :
 		
 			if not row[ 'words' ] : words = 0
 			else                  : words = row[ 'words' ]
+			
+			# using try is a hack; need to fix this
 			#records.append( int( row[ 'words' ] ) )
-			records.append( int( words ) )
+			try : records.append( int( words ) )
+			except ValueError : continue
 		df = pd.DataFrame( records, columns=COLUMNS )
 
 		# initialize the plot
 		figure, axis = plt.subplots()
 		
 		# plot
 		if output == 'histogram' : 
@@ -2383,15 +2841,16 @@
 	# output; csv
 	if output   == 'csv' : return( rows.to_csv() )
 	
 	# tsv
 	elif output == 'tsv' : return( rows.to_csv( header=False, sep='\t' ) )
 	
 	# json
-	elif output == 'json' : return( rows.to_json( orient='records' ) )
+	#elif output == 'json' : return( rows.to_json( orient='records' ) )
+	elif output == 'json' : return( rows.to_json( orient='index' ) )
 	
 	# count; tsv stream of metadata
 	elif output == 'count' :
 	
 		# build
 		results = COUNT.replace( '##CARREL##', carrel )
 		results = results.replace( '##QUERY##', query )
@@ -2693,19 +3152,19 @@
 	output      = localLibrary/carrel/PROVENANCE
 	with open( output, 'w', encoding='utf-8' ) as handle : handle.write( '\t'.join( record ) + '\n' )
 	
 	# process each item in the given directory
 	directory = Path( directory )
 	for source in directory.glob( '*' ) :
 
-		# check for metadata file
-		if source.name == METADATA :
+		# check for metadata file; look for a very specific file
+		if source.name == 'metadata.csv' :
 		
 			# copy the metadata file to the root of the carrel
-			destination = localLibrary/carrel/( source.name )
+			destination = localLibrary/carrel/METADATA
 			shutil.copyfile( source, destination )
 
 		else :
 		
 			# copy the file to the cache directory
 			destination = localLibrary/carrel/CACHE/( source.name )
 			shutil.copyfile( source, destination )
@@ -3351,36 +3810,37 @@
 	try to install it on your behalf. If the given directory contains a file
 	named 'metadata.csv', then this command will use the file as the source
 	of author, title, and date metadata values. This is often very helpful
 	because sans metadata it is very difficult to make comparison between
 	documents. Please see the full-blown documentation for details."""
 
 	# configure
-	CACHE  = 'cache'
-	TXT    = 'txt'
-	SCHEMA = '''-- parts-of-speech\ncreate table pos (\n    id    TEXT,\n    sid   INT,\n    tid   INT,\n    token TEXT,\n    lemma TEXT,\n    pos   TEXT\n);\n\n-- name entitites\ncreate table ent (\n    id     TEXT,\n    sid    INT,\n    eid    INT,\n    entity TEXT,\n    type   TEXT\n);\n\n-- keywords\ncreate table wrd (\n    id      TEXT,\n    keyword TEXT\n);\n\n-- email addresses\ncreate table adr (\n    id      TEXT,\n    address TEXT\n);\n\n-- questions\ncreate table questions (\n    id       TEXT,\n    question TEXT\n);\n\n-- urls\ncreate table url (\n    id     TEXT,\n    domain TEXT,\n    url    TEXT\n);\n\n-- bibliographics, such as they are\ncreate table bib (\n    id        TEXT,\n    words     INT,\n    sentence  INT,\n    flesch    INT,\n    summary   TEXT,\n    title     TEXT,\n    author    TEXT,\n    date      TEXT,\n    txt       TEXT,\n    cache     TEXT,\n    pages     INT,\n    extension TEXT,\n    mime      TEXT,\n    genre     TEXT\n);'''
-	POS    = 'pos'
-	ENT    = 'ent'
-	WRD    = 'wrd'
-	ADR    = 'adr'
-	URL    = 'urls'
-	BIB    = 'bib'
-	POOL   = 48
+	CACHE     = 'cache'
+	TXT       = 'txt'
+	SCHEMA    = '''-- parts-of-speech\ncreate table pos (\n    id    TEXT,\n    sid   INT,\n    tid   INT,\n    token TEXT,\n    lemma TEXT,\n    pos   TEXT\n);\n\n-- name entitites\ncreate table ent (\n    id     TEXT,\n    sid    INT,\n    eid    INT,\n    entity TEXT,\n    type   TEXT\n);\n\n-- keywords\ncreate table wrd (\n    id      TEXT,\n    keyword TEXT\n);\n\n-- email addresses\ncreate table adr (\n    id      TEXT,\n    address TEXT\n);\n\n-- questions\ncreate table questions (\n    id       TEXT,\n    question TEXT\n);\n\n-- urls\ncreate table url (\n    id     TEXT,\n    domain TEXT,\n    url    TEXT\n);\n\n-- bibliographics, such as they are\ncreate table bib (\n    id        TEXT,\n    words     INT,\n    sentence  INT,\n    flesch    INT,\n    summary   TEXT,\n    title     TEXT,\n    author    TEXT,\n    date      TEXT,\n    txt       TEXT,\n    cache     TEXT,\n    pages     INT,\n    extension TEXT,\n    mime      TEXT,\n    genre     TEXT\n);'''
+	POS       = 'pos'
+	ENT       = 'ent'
+	WRD       = 'wrd'
+	ADR       = 'adr'
+	URL       = 'urls'
+	BIB       = 'bib'
+	POOLSMALL = 48
+	POOLBIG   = 54
 	
 	# require
 	from   multiprocessing import Pool
 	import os
 	import shutil
 	import sqlite3
 	import pandas as pd
 	import spacy
 	
 	# _initialize
 	localLibrary = configuration( 'localLibrary' )
-	pool         = Pool( POOL )
+	pool         = Pool( POOLSMALL )
 
 	# make sure we have Tika Server
 	_checkForTika( str( configuration( 'tikaHome' ) ) )
 	
 	# start tika; the toolbox's secret sauce
 	if start :
 	
@@ -3457,15 +3917,15 @@
 		pool.starmap( _file2bib, [ [ carrel, filename, metadata ] for filename in filenames ] )
 		
 	# no metadata file; just do the work
 	else : pool.starmap( _file2bib, [ [ carrel, filename ] for filename in filenames ] )
 		
 	# clean up
 	pool.close()
-	pool = Pool( POOL )
+	pool = Pool( POOLBIG )
 
 	# bag of words
 	click.echo( '(Step #3 of 9) Creating bag-of-words', err=True )
 	_txt2bow( carrel )
 	
 	# output hint
 	click.echo( ( "\n  Hint: Now that the bag-of-words has been created, you can begin\n  to use many of the other Reader Toolbox commands while the\n  building process continues. This is especially true for larger\n  carrels. Open a new terminal window and try:\n\n    rdr cluster %s\n    rdr ngrams %s -c | more\n    rdr concordance %s\n    rdr collocations %s\n" % ( carrel, carrel, carrel, carrel ) ), err=True )
@@ -3477,39 +3937,39 @@
 
 	# extract email addresses
 	click.echo( '(Step #4 of 9) Extracting (email) addresses', err=True )
 	pool.starmap( _txt2adr, [ [ carrel, filename ] for filename in filenames ] )
 	
 	# clean up
 	pool.close()
-	pool = Pool( POOL )
+	pool = Pool( POOLBIG )
 
 	# extract named entities
 	click.echo( '(Step #5 of 9) Extracting (named) entities', err=True )
 	pool.starmap( _txt2ent, [ [ carrel, filename ] for filename in filenames ] )
 	
 	# clean up
 	pool.close()
-	pool = Pool( POOL )
+	pool = Pool( POOLBIG )
 
 	# extract parts-of-speech
 	click.echo( '(Step #6 of 9) Extracting parts-of-speech', err=True )
 	pool.starmap( _txt2pos, [ [ carrel, filename ] for filename in filenames ] )
 
 	# clean up
 	pool.close()
-	pool = Pool( POOL )
+	pool = Pool( POOLBIG )
 
 	# extract urls
 	click.echo( '(Step #7 of 9) Extracting URLs', err=True )
 	pool.starmap( _txt2url, [ [ carrel, filename ] for filename in filenames ] )
 
 	# clean up
 	pool.close()
-	pool = Pool( POOL )
+	pool = Pool( POOLBIG )
 
 	# extract keywords
 	click.echo( '(Step #8 of 9) Extracting (key) words', err=True )
 	pool.starmap( _txt2wrd, [ [ carrel, filename ] for filename in filenames ] )
 
 	# clean up
 	pool.close()
```

### Comparing `reader-toolbox-0.2.2/rdr/rdr.py` & `reader-toolbox-0.2.3/rdr/rdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # rdr.py - a command-line interface for building and modeling Distant Reader study carrels
 
 # Eric Lease Morgan <emorgan@nd.edu>
 # (c) University of Notre Dame; distributed under a GNU Public License
 
 # July 30, 2021 - in Three Oaks with Pat; first real working version
 # June 14, 2022 - trying to consolidate everything into a single file
+# May  29, 2023 - whoefully lacking in updates here; added... everthing
 
 
 
 # constants for topic modeling
 MODELDIR        = 'etc/topic-model'
 VECTORS         = 'model.vec'
 TXT2VEC         = "%s/bin/mallet import-dir --input %s --output %s --keep-sequence TRUE --stoplist-file %s"
@@ -25,15 +26,14 @@
 TOPICS          = 'topics.tsv'
 LABELS          = [ 'docId', 'file' ]
 
 
 # require
 from rdr import *
 
-#####
 
 def _makeSummary( keys, header ) :
 
 	# require
 	import pandas as pd
 
 	# read and sort keys file
@@ -267,15 +267,15 @@
 	"""Output a brief description and version number of the Reader Toolbox (rdr) application."""
 
 	# configure
 	ABOUT = '''
   The Reader Toolbox (rdr) is a Python library and command-line
   application used to create and model data sets called Distant
   Reader study carrels. It was written and is maintaned by Eric
-  Lease Morgan <emorgan@nd.edu>. This is version 0.2.2.
+  Lease Morgan <emorgan@nd.edu>. This is version 0.2.3.
 '''
 
 	# do the work and done
 	click.echo( ABOUT )
 
 
 # addresses
@@ -356,14 +356,41 @@
 	* rdr cluster %s
 	* rdr ngrams %s -s 2 -c
 	* rdr wrd %s -c
 	* rdr tm %s
 ''' ) % ( carrel, carrel, carrel, carrel, carrel, carrel, ), err=True )
 
 
+# archive
+@click.command( options_metavar='[<options>]' )
+@click.argument( 'carrel', metavar='<carrel>' )
+def cmdZip( carrel ) :
+
+	"""Create an archive (index.zip) file of <carrel>"""
+			
+	# do the work and give a hint
+	carrel2zip( carrel )
+	click.echo('''\n  Done. An archive file (index.zip) has been created and saved
+  in the root of the ''' + carrel + ''' study carrel. Share the file
+  with your friends and colleagues.\n''', err=True )
+
+
+# reconcile, create RDF, and graph
+@click.command( options_metavar='[<options>]' )
+@click.argument( 'carrel', metavar='<carrel>' )
+@click.option('-v', '--save', is_flag=True, help='write output to default location')
+@click.option('-o', '--output', default='gml', help='gml for custom visualization (recommended); chart for graphic', type=click.Choice( [ 'gml', 'chart' ] ) )
+def cmdRDFGraph( carrel, output, save ) :
+
+	"""Create RDF (Linked Data) file against <carrel>"""
+			
+	# do the work
+	graph2gml( carrel, output, save )
+
+
 # catalog
 @click.command( options_metavar='<options>' )
 @click.option('-h', '--human', is_flag=True, help='output in a more human-readable form')
 @click.option('-l', '--location', default='local', type=click.Choice( [ 'local', 'remote' ] ), help='output in a more human-readable form')
 def cmdCatalog( human, location ) :
 
 	"""List study carrels
@@ -1243,15 +1270,16 @@
 
 @click.command( options_metavar='<options>' )
 @click.option('-p', '--process', default='model', type=click.Choice( [ 'model', 'read' ] ), help="type of work to do" )
 @click.option('-t', '--topics', default=8, help="number of topics to generate" )
 @click.option('-w', '--words', default=8, help="number of words used to describe topic" )
 @click.option('-i', '--iterations', default=2400, help="number of times to cacluate" )
 @click.option('-o', '--output', default='summary', type=click.Choice( [ 'summary', 'chart', 'topdocs', 'csv' ] ), help="type of report" )
-@click.option('-f', '--field', type=click.Choice( [ 'author', 'title', 'date', 'track', 'category', 'type', 'year', 'journal', 'topic' ] ), help="field for pivoting" )
+@click.option('-f', '--field', type=click.Choice( [ 'author', 'title', 'date', 'track', 'category', 'type', 'year', 'journal', 'topic', 
+'pub_place' ] ), help="field for pivoting" )
 @click.option('-y', '--type', default='pie', type=click.Choice( [ 'pie', 'bar', 'barh', 'line', 'scatter' ] ), help="type of chart" )
 @click.argument( 'carrel', metavar='<carrel>' )
 def cmdTm( carrel, process, topics, words, iterations, output, field, type ) :
 
 	"""Apply topic modeling against <carrel>
 	
 	Topic modeling is the process of enumerating latent themes from a corpus, and it is yet another way to describe a corpus's aboutness. It is suggested you start out small when it comes to the values for -t and -w. Repeat the modeling process and gradually increase the values. Increase the value of -i as the size of your carrel increases. Remember, there is no such thing as the correct value of -t. After all, exactly how many things are the sum of Shakespeare's works about?
@@ -1515,22 +1543,24 @@
 rdr.add_command( cmdGet,           name='get' )
 rdr.add_command( cmdGrammars,      name='grammars' )
 rdr.add_command( cmdInfo,          name='info' )
 rdr.add_command( cmdNgrams,        name='ngrams' )
 rdr.add_command( cmdNotebooks,     name='notebooks' )
 rdr.add_command( cmdPlay,          name='play' )
 rdr.add_command( cmdPos,           name='pos' )
+rdr.add_command( cmdRDFGraph,      name='rdfgraph' )
 rdr.add_command( cmdRead,          name='read' )
 rdr.add_command( cmdReadability,   name='readability' )
 rdr.add_command( cmdSearch,        name='search' )
 rdr.add_command( cmdSemantics,     name='semantics' )
 rdr.add_command( cmdServer,        name='web' )
 rdr.add_command( cmdSet,           name='set' )
 rdr.add_command( cmdSizes,         name='sizes' )
 rdr.add_command( cmdSql,           name='sql' )
 rdr.add_command( cmdSummarize,     name='summarize' )
 rdr.add_command( cmdTm,            name='tm' )
 rdr.add_command( cmdUrl,           name='url' )
 rdr.add_command( cmdWrd,           name='wrd' )
+rdr.add_command( cmdZip,           name='zip' )
 
 # do the work
 if __name__ == '__main__' : rdr()
```

### Comparing `reader-toolbox-0.2.2/rdr/server.py` & `reader-toolbox-0.2.3/rdr/server.py`

 * *Files identical despite different names*

### Comparing `reader-toolbox-0.2.2/reader_toolbox.egg-info/PKG-INFO` & `reader-toolbox-0.2.3/reader_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reader-toolbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: A command-line interface for creating and interacting with Distant Reader data sets (a.k.a. study carrels)
 Home-page: https://github.com/ericleasemorgan/reader-toolbox
 Author: Eric Lease Morgan
 Author-email: emorgan@nd.edu
 Project-URL: Bug Tracker, https://github.com/ericleasemorgan/reader-toolbox/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `reader-toolbox-0.2.2/setup.cfg` & `reader-toolbox-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reader-toolbox
-version = 0.2.2
+version = 0.2.3
 author = Eric Lease Morgan
 author_email = emorgan@nd.edu
 description = A command-line interface for creating and interacting with Distant Reader data sets (a.k.a. study carrels)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ericleasemorgan/reader-toolbox
 project_urls = Bug Tracker = https://github.com/ericleasemorgan/reader-toolbox/issues
```

### Comparing `reader-toolbox-0.2.2/setup.py` & `reader-toolbox-0.2.3/setup.py`

 * *Files identical despite different names*

