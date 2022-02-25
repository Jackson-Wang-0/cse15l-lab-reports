# **Lab Report 4 - Week 8**
### _By: Zhicheng Wang, Pid: A16869487_

![ChMkJlbKw0WIcjXGAA--xnhwdi4AALG0QOAIDAAD77e961](https://user-images.githubusercontent.com/97211608/155808012-ab2fc7c3-5efb-4e53-80fe-2c25455232c5.jpg)

## Snippet 1 
```
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)
```
## VScode preview of Snippet 1

<img width="326" alt="截屏2022-02-25 下午1 52 26" src="https://user-images.githubusercontent.com/97211608/155808129-19048715-b67f-4cd9-b3c4-d1a1b8355825.png">

- According to VScode, the last three lines count as links while the first doesn't

## Turning Snippet 1 into test 
```
 @Test
 public void testSnippet1() throws IOException {
      Path fileName = Path.of("snippet1.md");
	    String contents = Files.readString(fileName);
      ArrayList<String> links = MarkdownParse.getLinks(contents);

      assertEquals(List.of("`google.com,","google.com","ucsd.edu"),links);

    }
```
### Screenshot in `MarkdownParseTest.java`

<img width="549" alt="截屏2022-02-25 下午2 02 37" src="https://user-images.githubusercontent.com/97211608/155809147-3408ed3c-34a7-41b6-80a6-88d7a06a538d.png">


### My implementation 

<img width="675" alt="截屏2022-02-25 下午2 06 04" src="https://user-images.githubusercontent.com/97211608/155809506-c522521e-be6f-4f58-9ebc-b2c90ad743cc.png">

_sadly it failed_ 

