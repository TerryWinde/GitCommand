# Live Templates

header
Add a header for the file
```
/**
* Create by terry on $DATE$
* 
* Description:
*
*/
```

newInstance
Creates an instance of the fragment with arguments
```
companion object {
    fun newInstance($args$): $fragment$ {
      val args = android.os.Bundle()
      $nullChecks$
      $addArgs$
      val fragment = $fragment$()
      fragment.arguments = args
      return fragment
    }
}
```
