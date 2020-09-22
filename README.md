import { BasePage } from "../pages/BasePage";

const page = new BasePage();

fixture`Home`.page(page.baseUrl);

test('Correct title displays', async t => {
    await t
        .expect(page.title.textContent)
        .eql("name game")
});

test('Attempts counter increments after selecting a photo', async t => {
    const initialAttemptsCount = Number(await page.attempts.textContent)
    
    await t.click(page.firstPhoto);

    const finalAttemptsCount = Number(await page.attempts.textContent);

    await t
    .expect(finalAttemptsCount)
    .eql(initialAttemptsCount + 1);
});
import { Selector } from 'testcafe';

fixture `NameGame`
    .page `http://www.ericrochester.com/name-game/`;

test('New Test', async t => {
    await t
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('div').withText('name game'))
        .drag(Selector('#gallery div').withText('5').nth(2), 3, 10, {
            offsetX: 92,
            offsetY: 46
        })
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('1'))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1'))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('1').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .click(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .click(Selector('#gallery div').withText('2').nth(2))
        .doubleClick(Selector('#gallery div').withText('3').nth(2))
        .click(Selector('#gallery div').withText('4').nth(2))
        .click(Selector('#gallery div').withText('5').nth(2))
        .expect('').eql()
        .expect('').notEql();
});
