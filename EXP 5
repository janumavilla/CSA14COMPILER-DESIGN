#include <stdio.h>
int main() {
    char c;
    int whitespace_count = 0;
    int newline_count = 0;
    FILE *fp = fopen("example.txt", "r");
    if (fp == NULL) {
        printf("Error: Could not open file.\n");
        return 1;
    }
    while ((c = fgetc(fp)) != EOF) {
        if (c == ' ' || c == '\t') {
            whitespace_count++;
        } else if (c == '\n') {
            newline_count++;
        }
    }
    printf("Number of whitespaces: %d\n", whitespace_count);
    printf("Number of newlines: %d\n", newline_count);
    fclose(fp);
    return 0;
}
