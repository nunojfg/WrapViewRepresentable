# WrapViewRepresentable
WrapViewRepresentable

Inspired by https://www.swiftbysundell.com/tips/inline-wrapping-of-uikit-or-appkit-views-within-swiftui/

Just add this to your ContentView

```
struct ContentView: View {
   @State private var searchTerm : String = ""

    var body: some View {
        ZStack {
            ...
            SearchBar(text: $searchTerm)
        }
    }
}
```
