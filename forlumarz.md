```mermaid
graph TD
    A[Start - Wprowadzenie] --> B(Sekcja 0: Twoje Dane - Wymagane);
    B --> C(Sekcja I: Podstawowe Informacje Biegowe - Wymagane);
    C --> D(Sekcja II: Poziom Wytrenowania i Parametry Fizjologiczne - Opcjonalnie);
    D --> E{Sekcja III: Pyt. 13 - Kontuzje/Problemy?};
    E -- Nie --> F(Sekcja IV: Technika Biegu - Opcjonalnie);
    E -- Tak --> G(Sekcja III: Szczegóły Kontuzji - Pyt. 13.1-13.4);
    G --> F;
    F --> H(Sekcja V: Dieta i Odżywianie - Opcjonalnie);
    H --> I(Sekcja VI: Zgody - Wymagane);
    I --> J[Zakończenie Formularza];

    %% Opisy etapów (do celów dokumentacji, nie są renderowane wprost w diagramie Mermaid, ale opisują co zawiera dany krok)
    class A, B, C, D, F, H, I, J, G section;
    class E decision;

    classDef section fill:#a2e0a2,stroke:#333,stroke-width:2px;
    classDef decision fill:#ffcccc,stroke:#333,stroke-width:2px;
