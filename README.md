# Create-Vec-u32-
fn count_permutation(shipments: &amp;Vec&lt;u32>) -> usize {     let n = shipments.len();     let total: u32 = shipments.iter().sum();      // Перевірка, чи можна рівномірно розподілити вантаж     if total as usize % n != 0 {         panic!("Неможливо розподілити вантаж рівномірно.");     }
